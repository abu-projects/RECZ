# Recz — Complete App Screens Prompt

Use this document to generate the **full Recz app** screen by screen in one unified product language.

## Product Direction
Design a premium mobile app called **Recz**: a recommendation-first social discovery product powered by **social trust + AI (Rexy)**. Every screen must support one of these goals:
- discover recommendations
- evaluate them with context and trust
- save / share / plan / try
- ask Rexy for help deciding

The design must stay consistent with the attached Recz HTML direction and the current visual system:
- dark immersive UI
- Apple-inspired clarity
- premium **Liquid Glass** surfaces
- deep blacks, layered blur, translucent cards, soft glows
- hot pink / rose primary accent with purple secondary energy
- rounded iPhone-native geometry
- elegant typography, minimal noise, rich hierarchy

Do **not** invent random new UI patterns. Keep the design system, navigation logic, interaction style, and component language consistent across the whole app.

---

## Visual Style Rules

### Overall look
- Apple-style premium mobile product
- dark background close to `#050505`
- translucent glass cards with blur and subtle white borders
- high depth using glow, gradient haze, and layered shadows
- strong edge contrast, soft internal highlights, refined spacing
- clean typography and polished alignment
- premium motion-ready composition, even in static mockups

### Core style tokens
- Primary accent: rose / pink gradient similar to `#f43f5e → #db2777`
- Secondary accent: purple glow for AI / aura / match / taste identity
- Background: near-black with soft rose and purple ambient blobs
- Glass panel: translucent white at very low opacity with strong blur and hairline border
- Border style: 1px subtle white border, occasionally tinted rose/purple for active state
- Radius: large rounded corners, especially 20–28px feeling
- Buttons: glass secondary buttons, bright pink gradient primary CTA buttons
- FAB: floating Rexy AI action, circular, glowing, always premium

### Component language from current HTML direction
Reuse the same UI DNA visible in the attached HTML-based design:
- glass header bars
- floating search
- layered recommendation cards
- full-bleed imagery with dark gradient overlays
- contextual chips
- bottom nav with glass tray and glowing center action
- rich profile hero and orbit-style taste identity visuals
- elegant modal overlays
- cinematic recommendation detail sheets

---

## Product Rules from Feature Checklist
Only include features supported by the checklist and system map.

### Core content and discovery
- recommendation posts across restaurants, movies, shows, books, travel, shopping, experiences
- personalized home feed from trusted circle
- like, comment, share, save
- explore discovery
- Rollz short-form video and photo carousel content
- text threads / chains

### AI and intelligence
- Rexy floating AI entry on major surfaces
- conversational AI recommendation flow
- contextual filters: budget, vibe, location, occasion, cuisine
- explainability: why this recommendation
- social proof: buddies saved / tried / liked
- “I’m bored” quick recommendation mode
- find similar / refine results
- vibe scanner / rec extraction where relevant

### social and planning
- buddy discovery and matching
- buddy profiles and activity
- direct messaging and recommendation sharing in chat
- lists / saved / tried / itineraries / planning
- events and collaborative planning when relevant

---

## Navigation Framework
Primary bottom navigation:
1. Home
2. Explore
3. Create
4. Rollz
5. Inbox

Persistent global layer:
- Floating Rexy AI button

Secondary destinations that appear through flow:
- Search
- Recommendation detail
- Comments / discussion
- Lists
- Buddy discovery
- Buddy profile
- Profile
- Settings
- Notifications / activity
- Event detail / planning
- Itinerary / plan detail

---

## Universal Recommendation Object Rules
Every recommendation card or recommendation-based screen should visibly support these elements when relevant:
- title / subject
- category
- image or media
- source or recommender
- reason/context
- social proof
- vibe / budget / occasion / location chips
- save
- add to list
- ask Rexy
- share
- mark tried
- open details

Recommendation UI should feel like the same object is reused across Home, Explore, Search, Rollz, Threads, Chat, Lists, and Profiles.

---

## Master Prompt for the Whole App
Design the full Recz mobile app in a consistent Apple-inspired Liquid Glass style. Use the same design language as the provided Recz HTML reference: near-black background, translucent glass cards, bright rose gradient accents, purple ambient AI glows, rounded corners, floating elements, premium bottom navigation, polished hierarchy, and cinematic recommendation cards. The app is recommendation-first and powered by social trust and Rexy AI. Do not remove existing core elements already present in the current design direction. Preserve the visual energy, glass treatment, accent behavior, and component logic, while covering the complete feature checklist and product flow.

Every screen should feel like part of the same premium product system. Every recommendation-related screen should expose clear decision actions: save, add to list, share, mark tried, open details, ask Rexy, or compare. Keep layouts mobile-native, clean, luxurious, and highly legible.

---

# Screen-by-Screen Prompts

## 01. Splash
**Purpose:** branded entry screen.
**Content:**
- centered glowing Recz app icon / logo
- subtle rose aura bloom behind logo
- short line: “Discover better through people you trust”
- minimal liquid loading bar near bottom
- no clutter

**Prompt:**
Create the Recz splash screen in a premium Apple Liquid Glass style. Use a deep black background with a soft rose glow behind the centered Recz icon. Add a tiny premium loading indicator near the bottom. Keep it minimal, elegant, cinematic, and luxurious.

---

## 02. Welcome / Onboarding Intro
**Purpose:** communicate contextual discovery value.
**Content:**
- full-screen lifestyle hero image
- dark gradient overlay
- large glass info card at bottom
- title about contextual discovery
- supporting text about mood, time, and trusted-circle recommendations
- progress indicator
- next arrow CTA

**Prompt:**
Design the onboarding intro screen with a full-bleed atmospheric lifestyle image, a dark cinematic overlay, and a large floating liquid-glass card anchored near the bottom. Show a bold headline about contextual discovery, short supporting copy, onboarding progress dots, and a glowing next CTA.

---

## 03. Login
**Content:**
- title and subtitle
- Apple login button
- Google login button
- divider
- email and password fields
- forgot password link
- primary login button
- bottom switch to sign up

**Prompt:**
Design the Recz login screen in the same dark Apple Liquid Glass style with translucent auth buttons, glass input fields, subtle ambient purple/rose glow, and a bright pink primary CTA.

---

## 04. Sign Up
**Content:**
- title and intro text
- Apple sign up
- Google sign up
- name, email, password fields
- create account button
- link to login

**Prompt:**
Design the Recz sign-up screen matching the login style, with premium glass form fields, elegant spacing, and a glowing pink create account button.

---

## 05. Interest Selection
**Purpose:** onboarding preferences.
**Content:**
- title: what’s your vibe
- step progress
- grid of rounded glass category cards
- selected states highlighted with rose tint and glow
- next button pinned near bottom

**Prompt:**
Design the Recz interest selection screen with a 2-column grid of glass cards for interests like cafes, cinema, travel, dining, museums, and more. Selected cards should use a rose accent tint and subtle glow. Keep the layout premium, airy, and iPhone-native.

---

## 06. Taste Details / Preferences
**Purpose:** collect context preferences.
**Content:**
- segmented controls / pills for taste setup
- vibe chips
- budget selection
- maybe sliders or toggles for preference nuance
- continue CTA

**Prompt:**
Design a premium onboarding preference screen where users refine their taste profile using liquid-glass segmented controls, chips, and polished selectors for vibe, budget, and discovery preferences.

---

## 07. Follow Friends / Discover Buddies Onboarding
**Purpose:** connect social trust layer.
**Content:**
- title and short explanation
- connect contacts CTA
- suggested buddies list
- follow actions
- continue button

**Prompt:**
Design an onboarding social-discovery screen where users connect contacts and discover buddies with similar taste. Show glass user cards with avatars, mutual signals, and follow buttons.

---

## 08. Home / For You
**Purpose:** main personalized recommendation feed.
**Content:**
- glass top header with profile, greeting, and context
- intent entry / smart prompt
- floating search
- mood system or quick filter chips
- quick picks / scan cards
- hero recommendation card
- social taste section
- people with your vibe section
- upgraded taste section
- event preview section
- birthday reminder / social trigger card
- inline Rexy module
- retention loop card
- glass bottom nav and floating create / Rexy logic

**Prompt:**
Design the Recz Home / For You screen as the hero of the whole app. Use a premium Apple Liquid Glass style with a fixed glass header, dynamic contextual greeting, floating search, mood chips, layered recommendation cards, social proof, buddy activity, people-with-your-vibe discovery, event previews, inline Rexy intelligence, and strong save / ask / share / open actions. Make the screen feel alive, editorial, and decision-first.

---

## 09. Home Bottom Sheet / Micro Planning Flow
**Purpose:** help convert discovery into action.
**Content:**
- bottom sheet over home
- options like save, add to list, plan tonight, ask Rexy, compare

**Prompt:**
Design a premium translucent planning bottom sheet that slides over Home and helps users convert a recommendation into an action such as save, add to list, compare, plan, or ask Rexy.

---

## 10. Rexy AI Assistant — Entry State
**Purpose:** global AI landing screen.
**Content:**
- AI header
- Rexy avatar or visual core
- greeting
- suggested prompt chips
- “I’m bored” instant action
- initial recommendation cards
- voice and text input dock

**Prompt:**
Design the Rexy AI entry screen in a premium futuristic glass style. Use purple and rose ambient glows, a conversational layout, suggested prompt pills, and clean recommendation cards. Include voice input, text input, and obvious quick-start actions like “I’m bored,” “Find dinner,” or “Best for now.”

---

## 11. Rexy AI Conversational Response
**Purpose:** richer AI recommendation conversation.
**Content:**
- conversation thread
- place header
- why it fits you section
- vibe / best time / pricing / crowd grid
- follow-up Q&A
- embedded action cards
- booking / plan suggestion flow
- persistent input bar

**Prompt:**
Design a detailed Rexy conversation screen showing explainable recommendations. Include why-this-fit logic, context chips, actionable cards, and a premium AI conversation experience that feels helpful, elegant, and highly interactive.

---

## 12. Explore
**Purpose:** broader discovery beyond home.
**Content:**
- floating search
- main Rexy block
- browse by mood
- category sections like travel destinations, books, experiences
- horizontally scrollable recommendation groups

**Prompt:**
Design the Explore screen with a floating search bar, strong category browsing, mood-based discovery, and editorial recommendation sections. Keep it glassy, immersive, and premium, with section cards and bold visual curation.

---

## 13. Search
**Purpose:** natural language and filtered search.
**Content:**
- search input
- smart suggestion block
- filter pills for budget, vibe, occasion, location
- results list with recommendation objects
- AI fallback block
- trending searches

**Prompt:**
Design the Recz search screen with a premium glass search input, context filters, recommendation results, and a smart Rexy fallback when search intent is vague. The screen should feel fast, refined, and recommendation-driven.

---

## 14. Recommendation Detail
**Purpose:** full evaluation screen for a recommendation.
**Content:**
- immersive hero media
- top nav controls
- bottom content sheet
- title, location, rating, badges
- social context quote or friend review
- social summary
- primary actions: save, add to list, ask Rexy, share, mark tried
- utility actions
- discussion preview
- more like this section

**Prompt:**
Design a cinematic recommendation detail screen with a full-bleed hero image and a luxurious glass content sheet. Include social proof, contextual reasons, action buttons, discussion preview, and related recommendations. It should feel like the most important decision screen in the app.

---

## 15. Comments / Discussion
**Purpose:** threaded discussion around a recommendation.
**Content:**
- header
- main comments
- nested replies
- reaction bar
- reply composer
- ability to save recommendation from discussion

**Prompt:**
Design a premium discussion screen for recommendation comments and threaded replies. Use liquid-glass bubbles, subtle hierarchy, and make it easy to reply, react, and move back into recommendation actions.

---

## 16. Rate / Review Screen
**Purpose:** post-visit contribution.
**Content:**
- target place info
- big rating component
- quick tags
- review text area
- submit CTA

**Prompt:**
Design a premium rating and review screen where the user can rate a place, pick vibe tags, and write a short review after trying it. Keep the UI elegant, simple, and reward-like.

---

## 17. Create Menu Overlay
**Purpose:** central creation entry.
**Content:**
- blur overlay over current screen
- three primary options: post, thread, Rollz
- close control

**Prompt:**
Design the create menu overlay as a luxurious glass modal that opens from the bottom nav center action. Present three main creation choices: recommendation post, thread, and Rollz.

---

## 18. Quick Snap — Camera
**Purpose:** fast capture flow.
**Content:**
- live camera style screen
- top controls
- Rexy hint
- capture frame
- mode pills
- shutter controls

**Prompt:**
Design a quick-snap camera screen for instant recommendation capture. Make it feel polished, dark, cinematic, and integrated with Rexy’s intelligence.

---

## 19. Quick Snap — Preview + Input
**Purpose:** review captured image and enrich it.
**Content:**
- captured media preview
- Rexy detection badge
- place confirm / override
- star rating
- vibe tags
- audience selector
- publish CTA

**Prompt:**
Design a quick-snap preview screen where Rexy detects the place vibe and helps the user turn a photo into a rich recommendation. Include rating, tags, audience, and a premium publish flow.

---

## 20. Quick Snap — Publish Confirmation
**Purpose:** success state.
**Content:**
- success icon
- insight pill
- social reward card
- next actions

**Prompt:**
Design a polished publish confirmation screen for quick snap, with a celebratory but premium success state, subtle glow, social reward feedback, and strong next-step actions.

---

## 21. Create Post
**Purpose:** structured recommendation publishing.
**Content:**
- location selector
- media upload
- rating module
- review / caption text
- context tags
- preview
- publish button

**Prompt:**
Design the Create Post screen as a premium structured publishing flow for recommendations. Keep fields elegant, modular, and highly visual. The user should add media, rating, context, and supporting text in a glass-first interface.

---

## 22. Publish Success
**Purpose:** success state after regular post creation.
**Content:**
- confirmation message
- social reward card
- next actions like view post, share, create list, return home

**Prompt:**
Design the publish success screen with rich micro-reward feedback, liquid-glass celebration UI, and next-step actions.

---

## 23. Create List
**Purpose:** quick list creation.
**Content:**
- cover upload
- title
- mood / purpose
- visibility
- collaborative toggle
- preview of added items
- create CTA

**Prompt:**
Design a create-list screen in the Recz style with glass inputs, cover picker, privacy settings, and collaborative options. The UI should feel polished and useful for planning, not just storage.

---

## 24. Create New List — Full Flow
**Purpose:** fuller list-building experience.
**Content:**
- cover image picker with suggestions
- list name
- description
- purpose tags
- privacy
- collaborative toggle
- add items via search or saved recs
- live preview card
- create CTA
- hidden success overlay

**Prompt:**
Design the full create-list flow with premium detail, allowing users to create a purposeful collection or itinerary with cover art, description, tags, privacy, collaboration, and recommended items.

---

## 25. List Detail
**Purpose:** open saved list / collection.
**Content:**
- hero cover
- creator info
- action buttons
- list items
- ask Rexy what to pick
- share / collaborate if applicable

**Prompt:**
Design a list detail screen with a rich hero cover, creator context, polished actions, and elegant stacked recommendation items. Keep it feeling like a decision-ready planning board.

---

## 26. Match / Taste Comparison
**Purpose:** compare a user with a buddy.
**Content:**
- orbit visualization
- shared interests layer
- social context layer
- AI suggestion card
- plan together CTA
- secondary actions

**Prompt:**
Design the taste comparison screen as a high-end visual experience with orbit-style taste identity graphics, overlap glows, shared interests, social context, and AI-powered suggestions for what the two users should do together.

---

## 27. Activity / Notifications
**Purpose:** social and recommendation activity hub.
**Content:**
- today section
- like, follow, match, birthday reminder, comment, save, contextual rec alert
- clear action affordances

**Prompt:**
Design a premium activity screen with grouped notifications, social updates, recommendation alerts, and contextual actions. Keep the hierarchy clear, warm, and glassy.

---

## 28. My Profile — Posts
**Purpose:** user identity and public recommendation presence.
**Content:**
- hero section
- top actions
- taste identity hero orbit system
- tabs
- add button
- grid of posts
- bottom nav

**Prompt:**
Design the main profile screen with a beautiful taste identity hero, premium glass profile header, stats, tabs, and a recommendation post grid. Make the profile feel personal, stylish, and socially credible.

---

## 29. My Profile — Lists
**Content:**
- same profile hero system
- list tab active
- add button for list creation
- list cards with delete or edit actions

**Prompt:**
Design the lists tab within the user profile using the same hero system and tab structure, but swap the content grid for rich collection cards.

---

## 30. My Profile — Plans
**Content:**
- same profile hero system
- plans tab active
- add button for plan creation
- plan cards, including shared plans

**Prompt:**
Design the plans tab within profile, showing upcoming and collaborative plans in a premium glass card format.

---

## 31. My Profile — Plan Detail
**Purpose:** itinerary / collaborative plan detail.
**Content:**
- top glass nav
- hero cover image and title
- info card and description
- participants section
- shared recommendations and voting
- Ask Rexy module

**Prompt:**
Design a detailed plan / itinerary screen with a cinematic hero, participants, shared rec voting cards, and an inline Rexy planner module. Keep it elegant and collaboration-ready.

---

## 32. Activity / Invitations in Profile
**Purpose:** invitations and collaborative updates.
**Content:**
- invitation card
- sender avatar
- plan preview
- accept / decline or action controls
- secondary activity cards

**Prompt:**
Design a premium invitations and activity screen tied to planning, using glass cards and clear collaborative actions.

---

## 33. Other User Profile
**Purpose:** see another user’s recommendations.
**Content:**
- hero section
- back button
- action buttons
- taste match card
- tabs
- their recommendations grid

**Prompt:**
Design another user’s profile screen with a premium hero, visible taste match logic, strong follow/message actions, and their recommendation content below.

---

## 34. Settings
**Purpose:** account, preferences, support.
**Content:**
- account section
- preference section
- support section
- logout row

**Prompt:**
Design the Settings screen in a clean Apple-inspired glass list style with grouped settings panels, subtle glow, and strong readability.

---

## 35. Help / About Features
**Purpose:** explain key product features.
**Content:**
- feature cards for Lists, Match, Rexy, Personalization, Friends Influence

**Prompt:**
Design a premium help and feature-education screen using elegant glass cards that explain Recz’s most important product concepts.

---

## 36. Logout Confirmation Modal
**Purpose:** modal over settings.
**Content:**
- blurred background
- dark overlay
- centered modal with icon, message, cancel and confirm buttons

**Prompt:**
Design a refined logout confirmation modal with a strong glass modal surface, subtle danger styling, and premium Apple-like spacing.

---

## 37. Friends / Social Hub
**Purpose:** manage social graph.
**Content:**
- fixed header
- tabs
- following section
- discover section
- bottom nav

**Prompt:**
Design a Friends / Social Hub screen where users view following, discover people, and manage their trusted circle. Use polished list cards and social overlap cues.

---

## 38. Friends — Empty State
**Purpose:** no friends yet.
**Content:**
- tabs
- empty state illustration / glass card
- call to discover buddies

**Prompt:**
Design the empty state for the Friends area with a premium, hopeful, beautifully minimal glass empty state and a strong discover-buddies CTA.

---

## 39. Friends — Discover Tab
**Purpose:** suggested users and filters.
**Content:**
- fixed header
- tabs
- search bar
- category / filter chips
- suggested people cards
- bottom nav

**Prompt:**
Design the Friends discover tab with glass search, filter chips, and premium suggested-user cards that show overlap, vibe, or recommendation compatibility.

---

## 40. Chat List
**Purpose:** inbox overview.
**Content:**
- header
- search
- active taste circles horizontally
- conversation list with unread, group, read, and rec-only conversations

**Prompt:**
Design the Recz inbox / chat list in a luxurious dark glass style. Include search, active users, conversation previews, and recommendation-aware conversation states.

---

## 41. Chat Conversation
**Purpose:** one-on-one messaging with recommendation sharing.
**Content:**
- header with avatar and match signal
- text messages
- received recommendation card
- voice message bubble with waveform
- plan card inline
- typing indicator
- input bar with share-rec and mic actions

**Prompt:**
Design the full chat conversation screen using premium liquid-glass message bubbles, inline recommendation cards, voice message UI, planning modules, and a polished input bar.

---

## 42. Voice Message Recording UI
**Purpose:** voice capture inside chat.
**Content:**
- dimmed chat background
- recording overlay
- timer
- live waveform
- controls for delete / hold / lock

**Prompt:**
Design the chat voice-recording overlay with a futuristic but elegant liquid-glass recording panel, animated waveform, timer, and tactile bottom controls.

---

## 43. Share Recommendation in Chat
**Purpose:** choose a recommendation to send.
**Content:**
- header
- search
- taste-matched suggestions header
- recommendation list with selected state
- list section source
- bottom input and send area

**Prompt:**
Design the share-recommendation-in-chat screen where users select a rec from suggestions or lists, add a message, and send it in a polished social flow.

---

## 44. Rollz Feed
**Purpose:** vertical swipeable short-form discovery.
**Content:**
- full-screen media
- glass overlay with title, recommender, reason, vibe chips
- like, comment, save, ask Rexy, share
- open recommendation CTA

**Prompt:**
Design the Rollz feed as a full-screen vertical swipe discovery experience with short-form video or photo carousel content. Keep all actions contextual and recommendation-first, not generic entertainment.

---

## 45. Rollz Comments / Interaction Layer
**Purpose:** reactions and deeper engagement on a Roll.
**Content:**
- current media context preserved
- comments drawer or sheet
- quick reactions
- save / open rec / ask Rexy shortcuts

**Prompt:**
Design the Rollz discussion layer as a premium overlay that preserves the media experience while enabling comments and recommendation actions.

---

## 46. Thread Feed / Threads List
**Purpose:** list of text chains and conversations.
**Content:**
- header
- new thread CTA
- text-first cards
- tags and linked rec previews

**Prompt:**
Design a threads list screen for text-based discussions using elegant glass post cards, subtle metadata, and linked recommendation previews.

---

## 47. Thread Detail
**Purpose:** full discussion chain.
**Content:**
- root post
- replies
- nested recommendation extraction or save from thread action
- reply composer

**Prompt:**
Design the thread detail screen with a premium text-first layout, clean hierarchy, recommendation references, and actions to save or convert useful replies into recommendations.

---

## 48. Create Thread
**Purpose:** new discussion creation.
**Content:**
- title / topic field
- body area
- tags / category / optional linked recommendation
- publish CTA

**Prompt:**
Design the create-thread screen in the same premium system, focused on text clarity, rich composition, and optional recommendation linking.

---

## 49. Events Feed / Event Discovery
**Purpose:** event discovery from the checklist.
**Content:**
- upcoming event cards
- interest/location filters
- buddy attendance signals
- save/share/open

**Prompt:**
Design an events discovery screen that fits the Recz system, showing curated hangouts, meetups, and activities with strong social proof and contextual recommendation framing.

---

## 50. Event Detail
**Purpose:** evaluate an event.
**Content:**
- cover image
- event date/time/location
- attendee summary
- RSVP controls
- share with buddies
- ask Rexy if this fits the user

**Prompt:**
Design a premium event detail screen with a cinematic hero, clean schedule information, social attendance signals, RSVP actions, and recommendation-style context.

---

## 51. Event Creation / Host Flow
**Purpose:** host meetup or group activity.
**Content:**
- event title
- location
- date and time
- invite buddies
- cover image
- RSVP settings
- publish CTA

**Prompt:**
Design a host-event flow in the Recz design system with rich glass inputs, date and location selectors, and buddy invite tools.

---

## 52. Saved / Quick Save Hub
**Purpose:** central save state.
**Content:**
- saved items
- quick save vs list organization
- sort / filters
- ask Rexy what to pick

**Prompt:**
Design the Saved screen as an elegant planning-first hub, not a plain bookmark list. Use recommendation cards, sort controls, and a clear path from save to decision.

---

## 53. Itinerary / Travel Plan Builder
**Purpose:** travel planning from checklist.
**Content:**
- itinerary title and cover
- day sections
- recommendation items inside days
- collaboration or sharing
- ask Rexy optimize route / pick next stop

**Prompt:**
Design a premium itinerary builder for travel recommendations, keeping the same liquid-glass design language and recommendation card system.

---

## 54. Buddy Discovery / Match Stack
**Purpose:** buddy matching.
**Content:**
- swipe-based user cards or premium stacked cards
- similarity cues
- mutual interests
- actions to connect or skip

**Prompt:**
Design the buddy discovery / matching screen in a premium Recz style, using glass stacked cards, similarity metrics, mutual taste cues, and strong visual personality.

---

## 55. AI Buddy / Insider Profile
**Purpose:** represent AI personas from the checklist.
**Content:**
- AI label clearly visible
- archetype info
- their posts / lists / Rollz
- CTA to ask this persona or follow their taste

**Prompt:**
Design an AI Buddy / Insider profile that clearly communicates the persona’s style while staying aligned with the Recz premium visual system and transparent AI labeling.

---

## 56. Notifications for Buddy Requests / Matches
**Purpose:** social growth alerts.
**Content:**
- new buddy requests
- match celebrations
- accept / reply / view profile actions

**Prompt:**
Design a notification screen or module for buddy requests and new matches in the same refined social trust design language.

---

## 57. Onboarding Empty States / Smart Guidance
**Purpose:** empty-state support.
**Content:**
- empty search state
- empty home state fallback
- AI-generated suggestions
- helpful CTAs

**Prompt:**
Design polished empty states across the product using subtle illustration, glow, clear explanation, and strong actions like Ask Rexy, Explore, or Follow Buddies.

---

## 58. Business / Creator Promo Card Surfaces
**Purpose:** optional monetization-ready surfaces from checklist.
**Content:**
- featured placement card style
- shoutout or promoted recommendation treatment
- clearly premium, not spammy

**Prompt:**
Design a premium sponsored / featured recommendation card pattern that fits Recz’s design system without breaking trust or elegance.

---

## 59. Premium Membership / Upsell
**Purpose:** premium feature entry.
**Content:**
- elite membership card
- benefits list
- premium glass hero
- CTA

**Prompt:**
Design a premium membership screen for Recz with a luxurious glass hero, elevated benefits presentation, and a refined upsell CTA consistent with the brand.

---

## 60. Universal Modal / Sheet System
**Purpose:** reusable overlays.
**Content:**
- share sheets
- save to list modal
- compare choices sheet
- mark tried confirmation
- ask Rexy mini sheet

**Prompt:**
Design a unified liquid-glass modal and bottom sheet system for Recz that can support share, save, compare, mark-tried, and mini-AI interactions.

---

# Final Output Rules for Any AI Tool
When generating these screens:
- maintain one unified Apple Liquid Glass design system
- preserve the same style, mood, and core component language as the attached HTML design direction
- keep recommendation as the center of the product
- use the same element patterns whenever the feature exists in the checklist
- do not add backend-dependent features that are not in the checklist
- keep flows connected: Home → Explore / Search / Rollz / Detail → Save / List / Rexy / Chat / Tried
- make all screens mobile-native and premium

# Deliverable Expectation
Generate all screens as a complete mobile app design system with consistent spacing, styling, card logic, navigation, and AI/social recommendation behavior.
