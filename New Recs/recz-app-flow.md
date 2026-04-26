# Recz App Flow Structure

## 1. Information Architecture

### Main Navigation

**Bottom Nav**
- `Home`: Personalized recommendation feed from trusted circle activity and relevant recommendations.
- `Explore`: Broader discovery through categories, search, and filtered recommendation browsing.
- `Create`: Entry point for creating structured recommendation posts.
- `Rollz`: Short-form vertical video discovery for quick recommendation browsing.
- `Inbox`: Direct messages and recommendation sharing in 1:1 chat.

**Floating Elements**
- `Rexy AI Button`: Persistent global button available across all primary and detail screens.
- `Quick Save / Tried Actions`: Embedded inside recommendation cards, not separate navigation.

### Core Sections
- `Discovery Core`: Home, Explore, Search, Rollz, recommendation detail surfaces.
- `Creation Core`: Structured recommendation creation, post publishing, thread participation.
- `Organization Core`: Saved items, Recz Lists, Tried state management.
- `Social Trust Core`: Buddy discovery, Buddy profiles, Buddy activity visibility.
- `AI Decision Core`: Rexy chat, contextual refinements, explainable suggestions.
- `Identity Core`: User profile, posts, lists, activity, stats.

## 2. Global Experience Rules

### Recommendation Objects Across the App
- Every content surface must resolve into a recommendation action: `save`, `view details`, `share`, `mark tried`, or `ask Rexy`.
- Recommendation posts use a consistent structured card model across Home, Explore, Search, Lists, Buddies, Chat shares, and profile.
- Each recommendation card should always show:
  - Recommendation title or subject
  - Category
  - Short reason or context
  - Source person or Buddy
  - Social proof signals
  - Immediate action controls
- Rollz and Threads are alternate content formats, but both must link back to a recommendation object or recommendation decision.

### Global Rexy Integration
- Rexy is available from every major screen via floating action button.
- Rexy can be launched with screen context:
  - From a recommendation: "Why this?" or "Find similar"
  - From Explore/Search: refine current results
  - From Lists: help choose what to do next
  - From Rollz: convert inspiration into saved recommendations
- Rexy responses always support action:
  - Save recommendation
  - Open recommendation detail
  - Add to list
  - Share in chat
  - Refine with filters

### Social Proof Rules
- Social proof must stay decision-oriented, not vanity-oriented.
- Show:
  - Which Buddies recommended or saved something
  - Buddy comments that add context
  - Tried status from trusted users where relevant
  - Lightweight engagement counts only if they help confidence
- Avoid making likes/comments the primary hierarchy; recommendation relevance and trust stay dominant.

## 3. User Journeys

### A. First-Time User Flow

#### Goal
Get a new user to relevant recommendations fast, with enough preference and social context to personalize discovery.

#### Flow
1. `Splash / Entry`
2. `Onboarding Intro`
3. `Interest Selection`
4. `Optional Context Preferences`
   - budget sensitivity
   - vibe preferences
   - location relevance
   - common occasions
5. `Buddy Discovery Prompt`
   - discover and match with Buddies early to seed trusted-circle recommendations
6. `First Personalized Home Feed`
7. `Rexy Nudge`
   - prompt first AI action such as "I'm bored" or "Find me something for tonight"
8. `First Save or First List Creation`

#### Success Outcome
- User sees immediately relevant recommendations.
- User understands Recz is for finding trusted recommendations, not general posting.
- User completes one action: save, ask Rexy, or view a Buddy/profile.

### B. Discovery Flow

#### Goal
Open app, browse efficiently, evaluate trust signals, and save or act quickly.

#### Flow
1. Open app into `Home`
2. Scan personalized recommendation feed
3. Open a recommendation card or interact inline
4. View social proof and context
5. Save to default saved area or specific Recz List
6. Continue via:
   - similar recommendations
   - Buddy profile
   - category page
   - Rexy refinement

#### Core Loop
Browse -> evaluate -> trust-check -> save/share/mark tried -> continue discovery

### C. Create Recommendation Flow

#### Goal
Make recommendation creation structured, fast, and useful for downstream discovery.

#### Flow
1. Tap `Create`
2. Choose content type:
   - recommendation post
   - thread / chain
   - Rollz
3. For recommendation posts, complete structured fields:
   - category
   - item or subject being recommended
   - reason for recommendation
   - context tags such as vibe, budget, location, occasion
4. Add optional supporting media if relevant to the chosen format
5. Preview recommendation card
6. Publish
7. Post becomes discoverable in Home, Explore, Profile, Search, and share surfaces

#### Creation Principle
Structure comes before expression. The post must remain actionable as a recommendation unit.

### D. Rollz Flow

#### Goal
Use short-form video to speed up inspiration and convert viewing into recommendation actions.

#### Flow
1. Open `Rollz`
2. Enter swipeable vertical feed
3. Watch short recommendation video
4. Interact:
   - like
   - comment
   - share
   - save
   - open source recommendation
   - ask Rexy for similar
5. Convert to action:
   - save to list
   - open detail
   - share in chat
   - mark as tried later from saved/list context

#### Conversion Rule
Rollz is not passive entertainment. Every clip should lead toward a recommendation decision.

### E. AI Flow (Rexy)

#### Goal
Help users move from vague intent to confident choice.

#### Flow
1. Trigger Rexy from floating button or contextual entry point
2. Ask naturally:
   - recommendation request
   - "I'm bored"
   - follow-up on visible recommendation
3. Rexy returns recommendations with explanation
4. User refines using context filters:
   - budget
   - vibe
   - location
   - occasion
5. User acts:
   - save
   - add to list
   - share in chat
   - open recommendation detail
   - ask "Why this?"

#### AI Principle
Rexy reduces decision friction, not just content volume.

### F. Social Flow (Buddies)

#### Goal
Use trusted people to improve discovery quality and confidence.

#### Flow
1. Open `Buddy Discovery`
2. Browse suggested Buddies
3. Match with Buddies
4. View Buddy profile
5. Inspect:
   - recommendations posted
   - saved or tried activity where visible
   - category tendencies
6. Engage:
   - open recommendation
   - comment
   - share in chat
   - use Buddy context in Home and Explore discovery

#### Social Principle
Buddies are not a follower graph. They are trust inputs for recommendation ranking and confidence.

### G. Save & Plan Flow

#### Goal
Turn discovery into organized intent and later action.

#### Flow
1. Save a recommendation from any surface
2. Choose:
   - quick save
   - save to Recz List
3. Open saved items or list view
4. Organize recommendations into lists
5. Revisit saved content later
6. Mark item as `Tried`
7. Use tried state to inform future recommendations and profile activity

#### Planning Principle
Saving should always be one tap; organizing can happen immediately or later.

## 4. Screen-by-Screen Flow

### Splash / Entry
- **Purpose**: Brand entry and route user into onboarding or returning-user discovery.
- **Key UI Sections**: brand mark, loading state, routing logic.
- **Primary Actions**: continue automatically.
- **Entry Points**: app launch.
- **Exit Paths**: Onboarding, Home.

### Onboarding
- **Purpose**: Set expectations that Recz is for trusted recommendation discovery.
- **Key UI Sections**: value framing, interest selection, context preference setup, Buddy seeding prompt.
- **Primary Actions**: select interests, set preferences, continue, discover Buddies.
- **Entry Points**: first app launch.
- **Exit Paths**: Home, Buddy Discovery, Rexy first prompt.

### Home (For You)
- **Purpose**: Personalized recommendation feed driven by trusted circle and relevance.
- **Key UI Sections**:
  - top bar with search entry
  - recommendation feed
  - Buddy activity snippets
  - lightweight category pivots
  - Rexy floating button
- **Primary Actions**: open recommendation, like, comment, share, save, open Buddy, ask Rexy.
- **Entry Points**: app launch, bottom nav, notifications/deep links.
- **Exit Paths**: Recommendation detail, Thread View, Buddy Profile, Search, Rexy AI Chat, List View, Chat.

### Explore
- **Purpose**: Expand beyond trusted-circle feed into broader recommendation discovery.
- **Key UI Sections**:
  - search bar
  - category browsing
  - active filters
  - recommendation result grid/list
  - trending or high-confidence recommendations only if still recommendation-led
- **Primary Actions**: browse categories, apply filters, open recommendation, save, ask Rexy.
- **Entry Points**: bottom nav, category links, search results.
- **Exit Paths**: Search, Recommendation detail, Rollz Feed, Thread View, Rexy AI Chat.

### Search
- **Purpose**: Help users find recommendations using natural language or category intent.
- **Key UI Sections**:
  - natural language search input
  - recent/relevant queries
  - filters for budget, vibe, location
  - results segmented by recommendation content type where useful
- **Primary Actions**: search, refine, open recommendation, save, ask Rexy from query.
- **Entry Points**: Home, Explore, Rexy handoff, deep link.
- **Exit Paths**: Recommendation detail, Profile, Buddy Profile, Rollz Feed, Rexy AI Chat.

### Rollz Feed
- **Purpose**: Fast-moving video-first recommendation discovery.
- **Key UI Sections**:
  - full-screen vertical video player
  - recommendation summary overlay
  - source user/Buddy attribution
  - quick actions stack
- **Primary Actions**: swipe, like, comment, share, save, open recommendation detail, ask Rexy.
- **Entry Points**: bottom nav, recommendation post, profile, explore.
- **Exit Paths**: Recommendation detail, Comment sheet, Profile, Rexy AI Chat, List save flow, Chat share flow.

### Create Post
- **Purpose**: Publish structured recommendation content in post, thread, or Rollz format.
- **Key UI Sections**:
  - content type selector
  - structured form fields
  - contextual tags/filters
  - preview
  - publish action
- **Primary Actions**: create recommendation post, create thread, create Rollz, preview, publish.
- **Entry Points**: bottom nav create, contextual prompts.
- **Exit Paths**: Published post detail, Profile, Home.

### Thread View
- **Purpose**: Support recommendation discussion and chains that deepen context.
- **Key UI Sections**:
  - parent topic or originating recommendation
  - threaded replies
  - recommendation references inside discussion
  - action bar
- **Primary Actions**: read, reply, open linked recommendation, save referenced recommendation, share.
- **Entry Points**: recommendation card, Explore, Profile, search results.
- **Exit Paths**: Recommendation detail, Profile, Chat share, Rexy AI Chat.

### List View
- **Purpose**: Organize saved recommendations into decision-ready collections.
- **Key UI Sections**:
  - list header
  - recommendation items
  - tried state markers
  - sort/filter controls if needed
- **Primary Actions**: open saved item, reorganize saved items, mark tried, share recommendation, ask Rexy what to pick.
- **Entry Points**: save flow, profile, saved area, chat-shared list context if applicable.
- **Exit Paths**: Recommendation detail, Rexy AI Chat, Chat, Profile.

### Buddy Discovery
- **Purpose**: Help users find and match with Buddies that improve recommendation trust.
- **Key UI Sections**:
  - suggested Buddies
  - matching actions
  - category affinity or recommendation overlap indicators
- **Primary Actions**: match with Buddy, open profile, inspect overlap.
- **Entry Points**: onboarding, Home, Explore, Profile.
- **Exit Paths**: Buddy Profile, Home, Explore.

### Buddy Profile
- **Purpose**: Show a person's recommendation taste and activity as a trust source.
- **Key UI Sections**:
  - profile header
  - recommendations
  - lists
  - visible activity
  - stats tied to recommendation behavior
- **Primary Actions**: view recommendations, open lists, inspect activity, share recommendation, start chat.
- **Entry Points**: Home feed, recommendation attribution, Buddy Discovery, search.
- **Exit Paths**: Recommendation detail, List View, Chat, Home.

### Profile
- **Purpose**: Centralize the user's recommendation identity.
- **Key UI Sections**:
  - profile header
  - posts
  - lists
  - activity
  - stats such as saves, likes, tried activity
- **Primary Actions**: open posts, open lists, review activity, manage saved decision history.
- **Entry Points**: avatar tap, bottom-nav-associated avatar entry if present, deep links.
- **Exit Paths**: Post detail, List View, Home, Explore, Create Post.

### Chat
- **Purpose**: Support 1:1 collaboration around recommendations.
- **Key UI Sections**:
  - conversation list or active thread
  - message composer
  - shared recommendation cards in chat
- **Primary Actions**: send message, share recommendation, open shared recommendation.
- **Entry Points**: bottom nav inbox, Buddy profile, share action.
- **Exit Paths**: Recommendation detail, Buddy Profile, Home.

### Rexy AI Chat
- **Purpose**: Turn user intent into explainable recommendations and actions.
- **Key UI Sections**:
  - conversation thread
  - suggested prompts
  - filter chips for budget, vibe, location, occasion
  - recommendation result cards
  - explanation panel for "Why this?"
- **Primary Actions**: ask for recommendations, refine, save, share, add to list, open recommendation.
- **Entry Points**: floating AI button, contextual "Ask Rexy", search handoff, list decision support.
- **Exit Paths**: Recommendation detail, List View, Chat, Home, Explore.

## 5. Cross-Feature Connections

### Posts Connect to Rollz
- A recommendation post can have a Rollz expression that acts as a faster discovery format for the same recommendation.
- Rollz should always resolve back to the underlying recommendation object for saving, sharing, and explanation.
- Users can move from detailed post context to quick video preview and back without losing action continuity.

### Threads Generate Recommendations
- Threads are not standalone conversation spaces; they should anchor around recommendation topics, follow-up advice, or comparison chains.
- Useful thread replies can surface referenced recommendations that become saveable recommendation objects.
- Threads deepen confidence when a user needs more context before acting.

### AI Enhances Every Interaction
- From Home: Rexy explains or broadens recommendations.
- From Explore/Search: Rexy narrows overwhelming result sets.
- From Rollz: Rexy translates inspiration into actionable recommendations.
- From Lists: Rexy helps choose what to try next.
- From recommendation details: Rexy answers "Why this?" and suggests alternatives.

### Buddies Influence Discovery
- Buddy actions are used as trust cues on recommendation cards.
- Buddy profiles act as curated discovery hubs.
- Matched Buddies improve Home personalization and increase confidence in Explore results.
- Shared recommendations in chat create another social discovery loop that still centers on recommendation action.

## 6. UX Strategy Notes

### How to Avoid Clutter
- Use one consistent recommendation card model across the app.
- Keep engagement controls secondary to recommendation context and save actions.
- Make content-type differences clear through layout, but keep actions consistent.
- Let Rexy live as a global entry point instead of duplicating AI widgets inside every screen.

### How to Guide Decision-Making
- Prioritize `why`, `who recommended it`, and `what to do next`.
- Put save, add-to-list, and explainability close to every recommendation.
- Show filters and refinements only when they reduce uncertainty.
- Surface Buddy trust cues before generic popularity signals.

### How to Maintain a Recommendation-First Experience
- Every screen must answer one of three questions:
  - What should I discover?
  - Why should I trust it?
  - What should I do with it now?
- Avoid feeds or messaging states that become generic social chatter without recommendation value.
- Keep creation structured so every post improves future discovery quality.
- Ensure Rollz, Threads, Chat, and Profiles all point back to recommendation action rather than attention loops.

## Recommended Primary Flow Spine

`Onboarding -> Home -> Recommendation Detail / Rollz / Explore -> Save or Add to List -> Rexy Refinement or Buddy Validation -> Chat Share or Mark Tried`

This keeps the product centered on recommendation discovery, decision support, and follow-through instead of generic browsing.
