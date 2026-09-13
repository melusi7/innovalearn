# LinguaLearn — Mobile App Interface Design

## Brand Identity

**App Name:** LinguaLearn  
**Tagline:** Speak the World  
**Color Palette:**
- Primary: `#4F46E5` (Indigo) — conveys intelligence, trust, and learning
- Secondary: `#10B981` (Emerald) — success, progress, growth
- Accent: `#F59E0B` (Amber) — energy, encouragement, streaks
- Background Light: `#F8F7FF` (Soft lavender white)
- Background Dark: `#0F0E1A`
- Surface Light: `#FFFFFF`
- Surface Dark: `#1A1928`
- Foreground Light: `#1E1B4B`
- Foreground Dark: `#EEF2FF`

---

## Screen List

| # | Screen | Purpose |
|---|--------|---------|
| 1 | Splash / Onboarding | Welcome, language selection, goal setting |
| 2 | Home Dashboard | Daily streak, recommended lessons, quick actions |
| 3 | Lessons Browser | Browse lesson categories and units |
| 4 | Lesson Detail | Step-by-step lesson content with exercises |
| 5 | Vocabulary Training | Flashcard-based vocabulary practice |
| 6 | Speech Practice | Microphone-based pronunciation practice with AI feedback |
| 7 | Quiz | Adaptive multiple-choice and fill-in-the-blank quizzes |
| 8 | Quiz Results | Score, review, and retry options |
| 9 | Progress Tracking | XP, streaks, accuracy charts, skill breakdown |
| 10 | AI Tutor Chat | Personalized AI conversation and lesson suggestions |
| 11 | Profile & Settings | User profile, language goals, theme, notifications |

---

## Primary Content and Functionality

### 1. Onboarding (3 slides + setup)
- Slide 1: App intro with illustration
- Slide 2: Choose target language (Spanish, French, German, Japanese, Mandarin, Arabic)
- Slide 3: Set daily goal (5 / 10 / 15 / 20 min)
- Stored locally in AsyncStorage

### 2. Home Dashboard
- Greeting with user name and streak flame icon
- Daily XP progress bar toward goal
- "Continue Learning" card (last lesson)
- Quick action buttons: Lessons, Vocabulary, Speech, Quiz
- AI Tip of the Day card
- Recent achievements badges

### 3. Lessons Browser
- Category grid: Basics, Greetings, Numbers, Food, Travel, Business
- Each category shows unit count and completion percentage
- Locked/unlocked state with progress ring

### 4. Lesson Detail
- Lesson header with title, difficulty badge, estimated time
- Step-by-step cards: Translation, Grammar note, Example sentences
- Audio playback for native pronunciation
- "Mark Complete" button with XP reward animation

### 5. Vocabulary Training
- Flashcard flip animation (front: target word, back: translation + example)
- Swipe right = know it, swipe left = review again
- Session summary: cards reviewed, accuracy rate
- Spaced repetition logic (due-date based)

### 6. Speech Practice
- Large microphone button with animated waveform
- Target phrase displayed prominently
- AI analysis: phoneme-level accuracy score
- Visual feedback: correct (green), needs work (amber), incorrect (red)
- Retry and next phrase controls

### 7. Quiz
- Multiple choice (4 options) and fill-in-the-blank
- Timer bar per question (30 seconds)
- Immediate feedback after each answer
- Adaptive difficulty: harder questions if performing well
- Progress indicator (Q 3/10)

### 8. Quiz Results
- Score card with grade (A–F)
- XP earned animation
- Breakdown: correct / incorrect / skipped
- Review wrong answers inline
- "Try Again" and "Next Quiz" buttons

### 9. Progress Tracking
- Streak calendar (GitHub-style heatmap)
- Total XP, lessons completed, words learned counters
- Weekly activity bar chart
- Skill radar chart: Listening, Speaking, Reading, Writing, Vocabulary
- Achievements gallery

### 10. AI Tutor Chat
- Chat interface with AI tutor avatar
- Personalized lesson recommendations based on weak areas
- Conversational practice in target language
- Grammar correction with explanations
- Quick reply chips for common queries

### 11. Profile & Settings
- Avatar, display name, target language
- Daily goal slider
- Notification reminders toggle
- Dark/light mode toggle
- App version info

---

## Key User Flows

### New User Onboarding
Splash → Onboarding Slide 1 → Slide 2 (pick language) → Slide 3 (set goal) → Home Dashboard

### Daily Learning Loop
Home → Lessons Browser → Lesson Detail → Complete → XP reward → Home (streak updated)

### Vocabulary Session
Home → Vocabulary Training → Flashcard swipe session → Session Summary → Home

### Speech Practice
Home → Speech Practice → Record → AI score → Retry or Next → Home

### Quiz Flow
Home → Quiz → 10 questions → Quiz Results → Review or Retry → Home

### AI Tutor Interaction
Home → AI Tutor Chat → Ask question / get recommendation → Navigate to suggested lesson

---

## Navigation Structure

**Bottom Tab Bar (5 tabs):**
1. Home (house.fill)
2. Lessons (book.fill)
3. Practice (mic.fill)
4. Progress (chart.bar.fill)
5. Profile (person.fill)

**Stack navigators within tabs:**
- Lessons tab: Lessons Browser → Lesson Detail
- Practice tab: Practice Hub → Vocabulary / Speech / Quiz → Results
- Progress tab: Progress Overview → Achievement Detail

---

## Typography

- Headings: System font bold, 28–32pt
- Subheadings: System font semibold, 18–22pt
- Body: System font regular, 15–16pt, line-height 1.5
- Labels/Captions: System font medium, 12–13pt

## Component Style

- Cards: rounded-2xl, shadow-sm, bg-surface, border border-border
- Buttons: rounded-full (primary), rounded-xl (secondary)
- Progress bars: h-2, rounded-full, bg-primary
- Badges: rounded-full, px-3 py-1, text-xs font-semibold
