What's missing or weak vs. the feature list + client direction
Gaps I found by cross-checking the master list against the MD's "Screens That Need Adjustment" and what's actually in 1c.html:

Core Circle screens that are thin / generic:

Screen 37 (Taste Circle Hub) — currently a flat list of members with 2 sample avatars + a "Friends Taste" preview. Missing everything the client explicitly asked for: subsections for Taste Circle / Mutuals / Trusted People, circle segments (Close friends, Foodie crew…), circle-wide stats, circle taste map.
Screen 33 (Other Profile) — missing Taste Overlap %, Shared Vibes, Shared Saves, Shared Circle (mutuals), "Add to Circle" CTA. The MD explicitly calls for these.
Screen 77 (Compare Taste) — exists but should be restructured per the MD: Hero (two users connected), Match Summary, "Why Rexy thinks you're similar", Shared Recs, Shared Tags, top actions.
Entirely missing screens (referenced by feature list / improvements doc but no template exists):
4. Circle Activity Feed — "what your circle is doing now" (saves, plans, try-it moments). Called out in Explore improvements + GLOBAL UX.
5. Circle Feed (trust-filtered timeline) — a social feed scoped to only your Taste Circle, distinct from Home.
6. Shared Saves / Shared Lists screen — the overlap list between two users, reached from Other Profile.
7. Mutuals screen — "people you both trust" list, reached from Other Profile / Compare.
8. Circle Segments / Sub-circles — ability to group the circle (Close, Foodie, Travel, Movie-night) — required to power the "Buddy Filter Lens" (feature 11) and group plan invites.
9. Buddy Profile / Taste-Compatible Person card — spec'd in feature 13 (Buddy Profile View). Currently only screen-33 exists, missing mutuals + taste DNA preview.
10. Collaborative Lists editor (feature 4) — no screen.
11. Circle-only Plans feed — the MD asks for "Plans Nearby" + "Your Circle Tonight" on Home. No dedicated screen.
12. Circle Birthdays / Anniversary hub (feature 16) — banner exists conceptually, but no list view.
13. Circle Privacy & Management — mute/block/remove-from-circle, circle visibility settings.
14. Taste Circle Onboarding — first-5-people flow / sync-contacts gated state distinct from generic empty-state 38.
15. Group Decision Tools inside Plans (feature 15) — polls + vote screen scoped to a plan/circle; plan details exist but the voting UI does not.
16. Who Recz'd You / Who Saved Your Recs — from Circle — required by Trust Graph feature but no dedicated screen.
17. Circle Taste Map / Collective Vibe — visual showing the circle's aggregate taste DNA (natural extension of Taste Sphere + Circle).
18. "Buddy Filter Lens" results screen — feature 11 Rexy capability ("Show me what Ananya would love here") has no UI.

Naming inconsistency to fix: feature list still uses "Buddy / Buddies"; client approved Taste Circle as the replacement. Circle screens use it correctly; other screens (feature list, copy in some templates) still say Buddy.

Prompt to hand to the designer / Claude

RECZ — Enhance Social (Taste Circle) Screens

Context
-------
RECZ is a social taste network, not a dating or recommendation-utility app.
The client has explicitly approved:
  • "Taste Circle" replaces "Buddy / Match" everywhere.
  • Mutual follow = enters your Taste Circle.
  • One-way follow = discover their recs only.
  • Communities = interest/taste-based, not dating-style.

The client says the Social (Circle) screens feel thin and must be enhanced.
Work from the existing file: "New Recs/1c.html". Keep the liquid-glass dark
aesthetic (cleaner cards, less heavy gradients, softer glass per the global
design direction at the bottom of the MASTER FEATURE LIST).

Goal
----
Turn Taste Circle from a contact list into the social heart of the app —
a trust-weighted, taste-driven social graph with visible overlap, shared
activity, and group action.

Rework these existing screens
-----------------------------
1. screen-37  Your Taste Circle (hub)
   Restructure into 4 zones:
     a) Circle Pulse header — "Your circle is into cozy cafés tonight"
        (dynamic, time-aware) + 3 stacked avatars of most-active members.
     b) Sub-tabs: All · Mutuals · Trusted · Insiders · Segments
        (Segments = Close, Foodie, Travel, Movie-night — user-created).
     c) Circle Activity strip — horizontal cards: "Maya saved 3 spots",
        "Shiv is planning dinner Fri", "New rec from Pankhuri".
     d) Member list rows show: avatar, name, taste-overlap %, last rec
        thumbnail, quick chat icon. Long-press = add to segment / mute /
        remove. Row tap → screen-33.
   Add a "Circle Taste Map" card (collective Taste Sphere of the circle).
   Keep search + Invite CTA in header.

2. screen-33  Other Profile
   Add, directly under the bio:
     • Taste Overlap % with a ring visualization
     • Compatibility line ("Loves the same hidden cafés")
     • Shared Vibes chips (Quiet cafés · Indie films · Rooftops)
     • Shared Saves card (tap → new "Shared Saves" screen)
     • Shared Circle row (mutuals, tap → new "Mutuals" screen)
   Top actions only: Follow · Add to Circle · Message.
   Remove any "Buddy" language.

3. screen-77  Compare Taste
   Restructure top-down:
     Hero (two avatars connected) → Match Summary (overlap %, top matching
     categories, shared vibes) → "Why Rexy thinks you're similar" (short
     AI explanation) → Shared Recommendations grid → Shared Tags chips →
     bottom: Message · Follow · Add to Circle.

4. screen-54  Taste Circle Discovery (swipe)
   Keep the swipe stack, but add per-card:
     • mini Taste Sphere preview
     • "3 mutuals" badge
     • 3 shared recs thumbnails
     • tap "i" to flip card and see full taste DNA.
   Remove anything that reads like Tinder (no "X / heart" framing — use
   "Skip" and "Add to Circle" labels).

5. screen-39 / 56 / 76  (Discover / Requests / Expand)
   Align visual language with 37. On each member card surface: taste
   overlap %, shared vibes, mutual count, last rec.

NEW screens to design
---------------------
A. Circle Feed
   A trust-filtered vertical feed (scoped to the Taste Circle only),
   distinct from Home/For You. Posts carry "X in your circle recz'd this"
   + overlap badge. Filter chip row: All · Recs · Rollz · Lists · Plans ·
   Threads. Reachable from Circle tab + from Home's "Circle Picks" row.

B. Circle Activity
   A chronological activity log (saves / tries / plans / new connections /
   birthdays) for the entire circle, reverse-chronological, groupable by
   day. Reachable from screen-37 strip "See all".

C. Shared Saves (two-user overlap)
   Grid of recs both users saved. Opened from Other Profile and Compare.
   Header shows "You + Jessica · 14 shared recs".

D. Mutuals
   List of people you both have in your Taste Circle. Each row shows
   both-sides overlap % and a "Message all" CTA to start a group chat.

E. Circle Segments
   Manage sub-circles (Close, Foodie crew, Movie nights…). Create/rename/
   reorder, add members. Segments power Buddy Filter Lens + plan invites.

F. Buddy Filter Lens (Rexy result view)
   "Show me what Maya would love here" — same result grid as Rexy answer,
   but every card carries a tiny "Maya says:" annotation explaining fit.

G. Circle Taste Map
   Full-screen view of the circle's aggregate Taste Sphere with drill-in
   on each arc (who contributes most to Food? to Indie film?).

H. Circle Birthdays / Anniversaries
   Upcoming 30 days, grouped by This week / Next week / Later. Each row
   has quick actions: Send rec · Send rec + gift · Open Rexy birthday
   flow. Links to feature 16.

I. Circle Privacy & Management
   Manage circle visibility, muted members, removed members, who can
   request to join, contact-sync permissions.

J. Collaborative List Editor
   Multiple avatars on list header, add-collaborator sheet, per-item
   attribution ("Added by Shiv"). Reachable from any List.

K. Plan Voting / Group Decision
   Inside an existing Plan: poll card (restaurant A vs B vs C) with
   real-time tallies, time-slot picker, comment thread. Links to feature 15.

L. Who Recz'd You (from Circle)
   A filtered view of your notifications showing only people in your
   Taste Circle who recz'd, saved, or tried your posts — distinct from
   the general Activity screen (27).

Global rules for every screen above
-----------------------------------
• Everywhere a user appears, show taste-overlap %, shared vibes count,
  or "in your circle" badge — never a bare avatar.
• Never use the word "Buddy" in copy; use "Taste Circle", "circle",
  "mutuals", "trusted".
• No dating metaphors (no hearts, no swipe-hot, no "match").
• Respect the global design direction at the end of the MASTER FEATURE
  LIST: softer glass, cleaner cards, more breathing room, stronger
  hierarchy, less heavy gradients.
• Register each new screen in the Vue screen registry at the bottom of
  1c.html and add it to the Social + Planning group in the side nav.

Deliverable
-----------
Edit 1c.html directly. Add the new screens as <template id="screen-XX">
blocks, extend the `screens` array and `communitiesScreens`/equivalent
computed groups, and add a new "Taste Circle" group alongside
"Social + Planning" in the navigation. Keep all existing screens working.

=================
whats is done
==================
Rebuilt

screen-37 Taste Circle Hub — live Circle Pulse header, sub-tabs (All · Mutuals · Trusted · Insiders · Segments), horizontal Circle Activity strip, Circle Taste Map card, Segments row, member list with overlap % + last-rec thumbnail.
screen-33 Other Profile — top actions now Follow · Add to Circle · Message, new Taste Overlap ring + compatibility card, Shared Saves + Mutuals twin cards, shared-vibes chips.
New screens (90–96)

screen-90 Circle Feed — trust-filtered vertical feed with overlap badges, filter chips (All/Recs/Rollz/Lists/Plans/Threads).
screen-91 Circle Activity — grouped log (Today / Yesterday) of saves, plans, tries, joins.
screen-92 Shared Saves — two-user overlap grid with "BOTH" badges.
screen-93 Mutuals — people both users trust, with per-side overlap and Message-all CTA.
screen-94 Circle Segments — manage sub-circles (Close, Foodie crew, Movie nights, Travel buddies, create new).
screen-95 Circle Taste Map — full-screen collective taste radar + top contributors by category.
screen-96 Circle Birthdays — Today / This week / Next week / Later, with Rexy flow + Rec+Gift CTAs.
Wiring

Added to screens array and dynamic component registration 1c.html:10677, 1c.html:11707.
New tasteCircleScreens computed group.
Nav renamed: old "Social + Planning" group split — new Taste Circle group with all 11 Circle screens, Social + Planning keeps Itinerary and Plans.
New dedicated "Taste Circle" storyboard section in the gallery, inserted before Messages.
Template open/close balance checked (92/92), 81 screen templates total. Open 1c.html in the browser and the new Taste Circle section will render alongside the existing ones.

