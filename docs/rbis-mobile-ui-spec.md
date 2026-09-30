# RBIS Learning Platform — Mobile App UI/TZ Specification

## 1. Project overview

Product name: RBIS Learning Platform

Type: Mobile application for students

Audience:
- School-level learners
- Preparation students
- Olympiad participants
- Competitive exam learners

Main goals:
- Learn through subject-based tests
- Solve open, closed, topic-based, and olympiad tests
- Track performance and weak topics
- Maintain motivation with badges, streaks, and rankings
- Participate in olympiad events with fair time control and server-based validation

Scope:
- Student mobile app only
- No admin panel included in this document
- Olympiad and test ecosystem are integrated into the student flow

## 2. Brand identity

Core color:
- HEX: #5f0521
- RGB: 95, 5, 33
- CMYK: 36%, 100%, 71%, 54%

Supporting colors:
- Black background: #090909
- White text: #F7F7F7
- Soft white: #EDEDED
- Burgundy accent 2: #8A1D3F
- Success green: #2FAE66
- Error red: #D94A5D
- Warning yellow: #F2B84B
- Blue CTA: #2F6FDB

Style direction:
- Premium academic / luxury school brand
- Dark mode dominant
- Burgundy as the identity color
- High contrast, elegant serif headline style
- Minimal modern interface with premium institutional tone

## 3. Visual identity and logo usage

Logo direction:
- Shield crest with academic symbolism
- Book / knowledge symbol at the top
- RBIS emblem with luxury educational feel
- Dark background with burgundy emblem
- Icon should feel institutional and prestigious

Use cases:
- Splash screen
- App icon
- Auth header
- Brand banner in home screen

## 4. Product structure

Main modules:
1. Onboarding
2. Authentication
3. Home
4. Subjects
5. Tests
6. Olympiads
7. Monitoring / analytics
8. Leaderboard
9. Profile
10. Notifications
11. Settings
12. Test flow
13. Results and review
14. Certificates / achievements

## 5. User flow

1. User installs app
2. Sees onboarding
3. Registers or logs in via phone, Google, or Telegram
4. Opens home screen
5. Selects subject or test
6. Starts test or olympiad
7. Answers questions with autosave
8. Sees results and review
9. Tracks performance from monitoring
10. Participates in leaderboard and achievements

## 6. Screens and detailed requirements

### 6.1 Splash screen
Purpose:
- Brand introduction
- App loading moment

Layout:
- Black background
- Centered RBIS logo / shield emblem
- Brand name appears after logo if needed

UI style:
- Minimal motion
- Slow fade in/out

### 6.2 Onboarding
Number of screens: 3

Screen 1 — Welcome
- Logo top center
- Title: “RBIS Learning Platform”
- Subtitle: “Bilimni sinash, rivojlantirish va musobaqalarga tayyorgarlik”
- Primary CTA: “Boshlash”

Screen 2 — Features
- 3 cards:
  - Fanlar bo’yicha testlar
  - Olimpiadalar va musobaqalar
  - Natija monitoringi
- Dots indicator

Screen 3 — Choose path
- 3 options:
  - Maktab / kurs
  - Olimpiada
  - Mustaqil tayyorgarlik
- Final CTA: “Kirish”

### 6.3 Authentication
Main auth screen
- Logo at top
- 3 login buttons:
  - Telefon raqam orqali
  - Google orqali
  - Telegram orqali
- New user CTA: “Ro’yxatdan o’tish”
- Secondary text: “Shartnoma va siyosatga roziman”

Phone method flow:
- Enter phone number
- Receive SMS code
- Verify code
- Continue to home

Google and Telegram flows:
- One-click social auth
- Minimal extra screens

### 6.4 Home screen
Header:
- Greeting: “Salom, [Name]”
- Notification bell icon
- Search icon

Top sections:
1. Upcoming tests / tasks
2. Daily challenge
3. Recent results
4. Olympiad block
5. Quick actions
6. Subject highlights

Card structure:
- Subject name
- Test type
- Time remaining / start time
- Questions count
- Difficulty level
- CTA button

Quick actions:
- Tests
- Subjects
- Olympiads
- Leaderboard
- Profile

### 6.5 Subject selection screen
Layout:
- Header: “Fanlar”
- Search bar
- Subject grid with cards

Subjects examples:
- Matematik
- Fizika
- Kimyo
- Biologiya
- Informatika
- O’zbek tili
- Ingliz tili
- Adabiyot
- Tarix
- Geografiya

Each subject card contains:
- Icon
- Subject name
- Number of tests
- Level
- Progress bar
- CTA: “Ko’rish”

Subpage filters:
- Ochiq testlar
- Mavzuli testlar
- Yopiq testlar
- Monitoring testlari
- Olympiad testlari

### 6.6 Test list screen
Tabs:
- Ochiq
- Mavzuli
- Yopiq
- Monitoring
- Saved

Each item card contains:
- Subject
- Test title
- Type
- Duration
- Questions count
- Difficulty
- Completion status
- Button: “Boshlash” / “Davom ettirish”

### 6.7 Test flow screen
Header:
- Timer at top
- Current question number
- Subject name
- Bookmark icon
- Close / leave warning

Question area:
- Question title
- Image / formula / chart if needed
- Answer options

Question types:
- Single choice
- Multiple choice
- True / false
- Fill in blank
- Matching

Bottom actions:
- Oldingi
- Keyingi
- Belgilash
- Saqlash
- Yakunlash

Behavior rules:
- Answers autosave after selection
- If app is closed, user resumes from saved progress
- If connection is lost, answer queue waits until connected
- Test timer is server-based, UI is just display
- User may review question list navigation

### 6.8 Test review / results screen
After test finish:
- Score summary
- Percentage
- Right/wrong count
- Time used
- Rank or level change

Tabs:
- Umumiy
- Xatolar
- Tahlil
- Savollar

Detailed result per question:
- Correct / incorrect status
- Explanation text
- Right answer highlighted
- Option review

### 6.9 Olympiad flow
Main olympiad screen:
- Cards with date, duration, difficulty, entry type
- Public or code-based registration
- Countdown label

Registration flow:
1. Rules screen
2. Consent checkbox
3. “Boshlashga tayyorman”
4. Demo / technical check

During olympiad:
- Server-time synchronized start
- Global countdown
- All participants start simultaneously
- App switch detection warning
- Multiple warnings lead to test termination
- Secure environment for fairness

Result page:
- Live leaderboard or final leaderboard
- Position ranking
- Certificate eligibility
- Appeal button to flag question issues

### 6.10 Monitoring / dashboard
Sections:
- Overall progress
- Subject mastery
- Weak topics
- Daily streak
- Accuracy graph
- Last 7 days performance

Charts:
- Circular progress rings
- Vertical bar charts
- Line graph
- Heat or grid analysis

Subject analysis example:
- Matematik: 78%
- Fizika: 64%
- Kimyo: 52%
- Ingliz tili: 81%

### 6.11 Leaderboard
Tabs:
- Umumiy
- Sinf
- Maktab
- Do’stlar

User rank card:
- Rank number
- Name
- Score
- Streak
- Medal or badge

### 6.12 Profile screen
Header:
- Avatar
- Username
- Class / school / region
- Level
- Streak count

Sections:
- Stat cards
- Achievements
- Certificates
- Saved questions
- Settings
- Invite friends

Achievements examples:
- 7 kun ketma-ket
- 100 ta test
- Olimpiada finalisti
- Top 10
- Mavzu bo’yicha 100% aniqlik

### 6.13 Notifications
List items:
- New test available
- Olympiad is starting soon
- Result published
- Daily challenge reminder
- Certificate ready

Design:
- Icon + title + timestamp + action button

### 6.14 Settings screen
Options:
- Profile editing
- Language selection
- Theme mode
- Font size
- Notification preferences
- Privacy / secure mode
- Help and support
- Log out

## 7. Recommended UI patterns

### Layout standards
- 16px or 18px spacing grid
- Cards with rounded corners
- Dark surfaces with burgundy edge accents
- Strong shadows only in selected cards
- Minimal clutter, high readability

### Typography
- Headings: serif or elegant academic font
- Body: modern sans-serif
- Numbers/timers: large bold sans
- Buttons: medium-bold uppercase or title case

### Buttons
- Primary: burgundy fill
- Secondary: dark grey fill
- Outline: burgundy border
- Danger: red / soft red

### Input fields
- 52–60px height
- Dark fill with subtle border
- Burgundy on focus

### Tabs and chips
- Compact, minimal chip layout
- Selected chip in burgundy or white text depending on theme

## 8. Technical requirements

### Time validation
- All olympiad and test deadlines must be controlled by server time
- Mobile clock should only be used for display, not verification
- Prevent cheating by changing phone time

### Auto-save and resume
- Save after each answer
- Save on app close
- Resume from saved state after reconnect

### Security
- Detect app switching and screen capture for tests
- Android FLAG_SECURE support
- One device per account for active test session
- Block sharing or answer leakage before final submission

### Offline support
- Only simple tests can be cached offline
- Olympiad tests must be online only
- Pending results sync when network returns

### Performance
- Cache test lists by subject
- Lazy-load question data
- Optimize image and formula rendering
- Support high concurrency for olympiad events

## 9. MVP scope

Must include for first release:
- Registration and profile
- Login via phone / Google / Telegram
- Subject selection
- Test list by type
- Timer and autosave
- Result and review screen
- Olympiad registration and synchronized start
- Leaderboard
- Push notifications

Post-MVP features:
- Advanced analytics
- AI-generated questions
- Detailed certificate management
- Friend challenge system
- More exam-security tools

## 10. Figma file structure recommendations

- 01_Style_Guide
- 02_Onboarding
- 03_Auth
- 04_Home
- 05_Subjects
- 06_Test_List
- 07_Test_Screen
- 08_Result
- 09_Olympiad
- 10_Leaderboard
- 11_Profile
- 12_Settings
- 13_Notifications
- 14_Components

## 11. Design prompt for AI / Figma

Copy-paste prompt:

“Create a premium dark-mode academic mobile app UI for RBIS Learning Platform. Use the brand color #5f0521 burgundy on black background, with luxury education aesthetic, institutional look, elegant serif typography, minimal modern interface, high contrast. Design a student app with onboarding screens, phone auth, Google and Telegram login options, home dashboard with upcoming tests and olympiads, subject list grid, test screen with bold timer, question list, answer options, save and next buttons, result screen with analytics, leaderboard, profile with achievements and certificates, notifications, settings, and monitoring dashboard. Include premium academic shields, book-inspired iconography, strong premium school identity. Use elegant layout, rounded cards, subtle shadows, clear CTAs, and modern mobile UX. Make it ready for Figma design handoff and AI-generated UI exploration.”

## 12. Recommended next step

Use this spec directly in Figma and ask AI to generate the first pass of screens page by page.

Best workflow:
1. Create screen-by-screen wireframe in Figma
2. Export design tokens
3. Ask AI to generate UI variations
4. Refine with actual product logic and app behavior
5. Prepare final handoff for development

## 13. Final concise summary

RBIS app should feel like a premium educational platform with academic authority. The strongest emotional cues are:
- Burgundy + black
- Shield / academic crest
- High trust / high status
- Dark theme for focus
- Minimal but rich education interface

This is exactly suitable for a student-focused platform that mixes:
- Tests
- Olympiads
- Monitoring
- Leaderboard
- Achievements
- Academic prestige

## 14. File status

This specification is prepared for Figma and AI design generation.

You can now use it in Figma or feed it to a design AI to generate full screens.

---

If you want, I can continue with the next step and produce:
- Screen-by-screen Figma page list with exact titles
- Full mobile app wireframe text layout
- AI prompt for each individual screen
- Final PDF-ready output version in a cleaner business-document format
