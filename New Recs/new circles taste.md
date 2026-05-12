# New Circles Taste
## Session Documentation — Taste Circle Enhancement

**File modified:** `1c.html`
**Session goal:** Enhance and expand the Social (Taste Circle) screens based on client feedback that "social screens need to be enhanced (circles)."

---

## Context & Direction

RECZ is a **social taste network**, not a dating app or recommendation utility.

The client approved:
- "Taste Circle" replaces all "Buddy / Match" language
- Mutual follow = enters your Taste Circle
- One-way follow = discover their recs only
- No dating metaphors anywhere (no hearts-as-like, no swipe-hot framing)
- Communities = interest/taste-based groups, not social matching

---

## REBUILT SCREENS

---

### Screen 37 — Your Taste Circle Hub
**Status:** Complete rebuild (was a basic flat list)

**What it was before:**
A simple list of 2 sample members with a "Friends Taste" mini-section and a Sync Contacts banner. No visual hierarchy, no social context, no activity.

**What it is now:**
The social heart of the app — a rich, layered hub with 6 distinct zones.

---

#### Zone 1 — Circle Pulse (top card)
A dynamic header card that answers: *"What is my circle into right now?"*

- **`• LIVE PULSE` badge** — animated ping dot signals real-time activity
- **`142 in your circle`** — total circle size at a glance
- **Dynamic headline** — e.g. "Your circle is into cozy cafés tonight" — AI-generated based on what the circle is currently saving/planning
- **Explanation line** — why the headline is true (which vibe tags are trending, which segment is driving it)
- **Stacked avatars** — shows the specific people behind the trend (personal, not algorithmic)
- **`Open feed` button** — deep-links to Circle Feed (screen-90)

> **Why it matters:** Turns a passive contact list into a live social signal. The user immediately sees the value of their circle without having to dig.

---

#### Zone 2 — Sub-tabs
Horizontal scrollable filter row:
- **All · 142** — everyone in the circle
- **Mutuals · 86** — people who follow back
- **Trusted · 24** — manually elevated members
- **Insiders · 12** — Recz Insider AI personas followed
- **Segments** — opens Circle Segments screen (94) via pink pill button with widget icon

---

#### Zone 3 — Circle Activity Strip
Horizontal scrollable activity cards showing what the circle is doing right now:

| Card type | What it shows |
|---|---|
| Saves card | "Maya saved 3 spots" with thumbnail grid |
| Plan card | "Shiv is planning Friday dinner" with join CTA |
| Try-It card | "Pankhuri tried Verve Patio" with quote |
| Join card | "Jessica added to your Circle" with profile CTA |

Each card has a timestamp, action icon (bookmark/calendar/check/user-plus), and a context label (overlap %, open status).

`See all` → Circle Activity screen (91)

---

#### Zone 4 — Circle Taste Map Card
A teaser card that previews the circle's collective taste DNA:
- Mini radar visualization with colored dots (rose/purple/emerald/amber)
- Shows top taste categories of the circle (Coffee · Indie film · Low-noise dinners · Late nights)
- Taps → full Circle Taste Map screen (95)

---

#### Zone 5 — Segments Quick Row
3-column grid showing the user's segment shortcuts:
- Close (heart icon, rose)
- Foodie crew (plate icon, amber)
- Movie nights (film icon, purple)
- `Manage` link → Circle Segments screen (94)

---

#### Zone 6 — Member List
Full member list with enriched rows. Each row shows:
- Avatar with online indicator dot
- Name + tier badge (TRUSTED / MUTUAL / INSIDER)
- Last rec preview (place name, time, category)
- Overlap % (large, prominent)
- Last rec thumbnail (right side)

Members sorted by overlap % descending. `See all 142 members` CTA at bottom → Expand Your Circle (76).

---

### Screen 33 — Other Profile
**Status:** Enhanced (was a basic profile with just Follow + Message)

**What was added:**

#### Taste Overlap Ring
- SVG ring visualization showing overlap % (e.g. 85%)
- Gradient stroke (rose → purple)
- Compatibility tagline: "Loves the same hidden cafés and low-key dinner counters"
- `Compare taste` link → Compare Taste screen (77)
- Shared vibe chips: Quiet cafés · Indie films · Late nights · Rooftops

#### Shared Saves + Mutuals cards (2-column grid)
**Shared Saves card:**
- 3 rec thumbnails
- "14 shared recs" count
- "Places you both saved" label
- Taps → Shared Saves screen (92)

**Mutuals card:**
- Stacked avatars of shared circle people
- "7 people in common" count
- "Your shared circle" label
- Taps → Mutuals screen (93)

#### Top Actions — changed from 2 to 3 buttons
| Before | After |
|---|---|
| Follow · Message | Follow · Add to Circle · Message |

`Add to Circle` is now a prominent rose-colored primary action — reinforcing that adding someone to your Taste Circle is the main social action on this screen.

---

## NEW SCREENS

---

### Screen 90 — Circle Feed
**What it is:** A trust-filtered vertical social feed scoped exclusively to the Taste Circle. Different from Home/For You which shows everyone.

**Filter chips:** All · Recs · Rollz · Lists · Plans · Threads

**Post types rendered:**
1. **Rec post** — with "3 in your circle recz'd" badge overlay on image, overlap % in author row, like/comment/save actions
2. **Plan from circle** — rose-tinted card, open join status, stacked avatars, `Join plan` CTA
3. **List post** — author + tier badge, 3-image thumbnail grid, list title and tagline
4. **Rollz post** — full aspect-ratio video card with play button, circle context in caption

**Key difference from Home feed:** Every post shows social proof tied specifically to the user's circle — overlap %, tier badges, circle save counts. It's trust-weighted, not algorithmic.

---

### Screen 91 — Circle Activity
**What it is:** A chronological activity log of everything happening in the Taste Circle — saves, tries, plans, joins — grouped by day.

**Filter chips:** All · Saves · Tries · Plans · Joins

**Activity types:**
| Icon color | Action |
|---|---|
| Rose | Saves, bookmarks |
| Rose | Plan creation |
| Emerald | Try-It moments |
| Purple | New circle joins |
| Amber | Published lists |

**Grouping:** Today / Yesterday sections with timestamps.

**Actions on rows:**
- Plan rows → `Join` button
- New join rows → `View` profile button

> **Why it matters:** Gives users a full picture of circle life beyond just the feed. Surfaces passive activity (saves, tries) that never shows up as posts.

---

### Screen 92 — Shared Saves
**What it is:** A two-user overlap screen showing all the places both the logged-in user and another person have saved. Reached from Other Profile (33) and Compare Taste (77).

**Header card:**
- Side-by-side avatars of both users
- "You + Sarah J. · 14 shared recs · 85% taste overlap"
- `Save list` CTA to export as a Recz List

**Filter chips:** All · 14 · Food · 6 · Coffee · 4 · Film · 3

**Content:** 2-column grid of rec cards with `BOTH` badge on each, place name, category/vibe tag.

---

### Screen 93 — Mutuals
**What it is:** A list of people that both the logged-in user AND another person have in their Taste Circles. Reached from Other Profile (33).

**Header card:**
- Side-by-side avatars
- "7 people you both trust"
- `Message all 7` primary CTA — one tap to start a group chat with all shared circle members

**Member rows:** Each row shows:
- Avatar + name
- "You: 94% · Sarah: 88%" — both-sides overlap at a glance
- `Message` individual CTA

---

### Screen 94 — Circle Segments
**What it is:** A management screen for sub-circles within the Taste Circle. Private organizational groups that power Rexy lens filters, plan invites, and scoped feeds.

> ⚠️ **Note:** This feature is NOT in the Master Feature List. It was added as part of this session's design gap analysis. **Needs client approval before shipping.**

**Each segment card shows:**
- Colored icon representing the segment type
- Segment name + member count + description
- Stacked avatars of members
- 3-dot menu (for rename/delete)

**Default segments designed:**
| Segment | Icon | Color |
|---|---|---|
| Close | Heart | Rose |
| Foodie crew | Plate | Amber |
| Movie nights | Film | Purple |
| Travel buddies | Route | Emerald |

**`+ Create new segment`** — dashed border button at bottom.

**`+` button in header** — creates new segment from top right.

**Powers:**
- Rexy Buddy Filter Lens (show me what my Foodie crew would love)
- Plan invites (invite only Movie nights segment)
- Scoped circle feeds

---

### Screen 95 — Circle Taste Map
**What it is:** A full-screen visualization of the Taste Circle's collective taste DNA. Shows the aggregate of all 142 members' saves, posts, and activity.

**Hero card:**
- "142 people · 6,204 saves" context line
- "Your circle's collective taste" headline
- AI summary: "Low-noise dinners, indie film, patio coffee, late nights. Strong bias toward intentional places over trending ones."
- Radar sphere visualization:
  - Outer rings (white/10 opacity)
  - Colored floating category tags at compass points
  - Colored glow dots at each category position
  - Center group icon

**Category breakdown:**
| Category | Share | Color |
|---|---|---|
| Coffee | 34% | Rose |
| Low-noise dinners | 28% | Emerald |
| Indie film | 22% | Purple |
| Late nights | 16% | Amber |

**Top contributors section:**
Each category lists the 2-3 circle members who contribute most to that category, with their avatars.

---

### Screen 96 — Circle Birthdays
**What it is:** An upcoming birthdays hub scoped to the Taste Circle, with contextual action buttons for each person.

**Today banner (if birthday today):**
- Full rose-gradient card with cake icon
- Person's avatar prominently displayed
- 3 action buttons: `Message` · `Send rec` · `Rec + gift` (primary rose CTA)

**Upcoming sections:**
- This week
- Next week
- Later this month

**Each birthday row shows:**
- Avatar + name + date + age (e.g. "Thursday · turning 28")
- For imminent birthdays: `Rexy flow` button (triggers birthday Rexy conversation)
- For future birthdays: `Remind me` button

> Connects to Feature 16 (Birthday & Anniversary Feature) in the Master Feature List.

---

## WIRING & NAVIGATION CHANGES

### Vue Screen Registry
All 7 new screens added to the `screens` array in the Vue app data:

```
screen-90  Circle Feed
screen-91  Circle Activity
screen-92  Shared Saves
screen-93  Mutuals
screen-94  Circle Segments
screen-95  Circle Taste Map
screen-96  Circle Birthdays
```

All 7 registered in the dynamic component loop.

### New Computed Group
`tasteCircleScreens()` added — renders these screens in order:
37 → 90 → 91 → 33 → 77 → 92 → 93 → 94 → 95 → 96 → 76 → 54 → 56 → 39 → 38

### Side Navigation Groups
Old structure:
```
Social + Planning: Taste Circle · Itinerary · Plans
```

New structure:
```
Taste Circle:
  Circle Hub (37) · Circle Feed (90) · Circle Activity (91)
  Segments (94) · Circle Taste Map (95) · Birthdays (96)
  Shared Saves (92) · Mutuals (93) · Expand Your Circle (76)
  Discovery Swipe (54) · Requests (56)

Social + Planning:
  Itinerary Builder (53) · Plans (49)
```

### New Storyboard Section
A dedicated **"Taste Circle"** storyboard section added in the gallery, inserted before the Messages section. Includes a descriptor:

> "The social heart of Recz — trust-filtered discovery, circle activity, shared overlap, and group planning. Built around mutual follow, taste overlap, and segments — never dating metaphors."

---

## CROSS-SCREEN NAVIGATION MAP

```
Screen 37 (Circle Hub)
├── Open feed → Screen 90 (Circle Feed)
├── See all (activity) → Screen 91 (Circle Activity)
├── Segments button → Screen 94 (Circle Segments)
├── Circle Taste Map card → Screen 95 (Circle Taste Map)
├── Birthday icon (header) → Screen 96 (Circle Birthdays)
├── Invite icon (header) → Screen 76 (Expand Your Circle)
└── Member row tap → Screen 33 (Other Profile)

Screen 33 (Other Profile)
├── Compare taste → Screen 77 (Compare Taste)
├── Shared Saves card → Screen 92 (Shared Saves)
├── Mutuals card → Screen 93 (Mutuals)
├── Add to Circle button → adds to circle (new action)
└── Circle stat → Screen 37 (Circle Hub)

Screen 90 (Circle Feed)
└── Join plan → Screen 52 (Plan Details)

Screen 91 (Circle Activity)
└── Join → Screen 52 (Plan Details)

Screen 92 (Shared Saves)
└── Compare icon → Screen 77 (Compare Taste)

Screen 93 (Mutuals)
└── Message all → Screen 40 (Message List)

Screen 96 (Circle Birthdays)
└── Rexy flow → Screen 10 (Rexy AI)
```

---

## DESIGN PRINCIPLES APPLIED

All new screens follow the global design direction from the Master Feature List:

| Rule | Applied |
|---|---|
| Softer glass | `bg-white/[0.035]` instead of heavy `bg-white/5` |
| Less heavy gradients | Subtle `from-rose-500/[0.14]` not solid fills |
| Cleaner cards | Single border, minimal shadow, no glow borders |
| More breathing room | `gap-3`, `space-y-2`, section `mb-5/6` |
| Stronger hierarchy | `text-[10px] uppercase tracking` labels before every section |
| No dating language | Zero use of "Buddy", "Match", hearts-as-like, swipe-hot |
| Taste Circle language | "circle", "mutuals", "trusted", "taste overlap" throughout |

---

## FEATURE LIST ALIGNMENT

| Screen | Master Feature List reference |
|---|---|
| 37 Circle Hub | Feature 13 — Buddy Matching & Social Graph |
| 90 Circle Feed | Feature 8 — Social Feed |
| 91 Circle Activity | Feature 27 — Notifications & Nudges |
| 92 Shared Saves | Feature 13 — Trust Graph |
| 93 Mutuals | Feature 13 — Buddy Matching |
| 94 Segments | ⚠️ NOT in Master Feature List — needs approval |
| 95 Taste Map | Feature 2 — Taste Identity / Feature 13 |
| 96 Birthdays | Feature 16 — Birthday & Anniversary Feature |

---

## OPEN ITEMS FOR CLIENT

1. **Circle Segments (screen-94)** — feature not in Master Feature List. Decision needed: approve and add to list, or remove from prototype.
2. **"Add to Circle" action** — added to Other Profile (33). Client to confirm this is the right primary CTA hierarchy vs. Follow.
3. **Circle Feed (90) vs Home Feed** — two distinct feeds now exist. Nav tab strategy to be confirmed (does Circle Feed live inside the Circle tab or as a separate tab?).
4. **Segments naming** — "Close", "Foodie crew", "Movie nights", "Travel buddies" are placeholder defaults. Client to define if defaults are auto-suggested or user-named only.
