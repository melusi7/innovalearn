# LinguaLearn TODO

## Onboarding & Setup
- [x] Onboarding flow (3 slides: intro, language selection, goal setting)
- [x] AsyncStorage persistence for user profile and preferences
- [x] Language selection screen (Spanish, French, German, Japanese, Mandarin, Arabic, Italian, Portuguese)
- [x] Daily goal setting (5/10/15/20 min)

## Home Dashboard
- [x] Greeting with streak flame and daily XP progress
- [x] Continue Learning card (last lesson shortcut)
- [x] Quick action buttons (Lessons, Vocabulary, Speech, Quiz)
- [x] AI Tip of the Day card
- [x] Recent achievements badges

## Lessons
- [x] Lessons browser with category grid
- [x] Category cards with completion percentage and lock state
- [x] Lesson detail screen with step-by-step cards
- [x] Mark Complete with XP reward animation

## Vocabulary Training
- [x] Flashcard component with flip animation
- [x] Spaced repetition logic (SM-2 algorithm)
- [x] Session summary with score

## Speech Practice
- [x] Microphone recording UI with animated waveform
- [x] AI speech analysis via backend LLM
- [x] Accuracy, fluency, rhythm score display
- [x] Visual feedback (green/amber/red)
- [x] Retry and next phrase controls

## Quizzes
- [x] Multiple choice quiz component
- [x] Timer bar per question
- [x] Quiz results screen with score and XP
- [x] Answer review with explanations

## Progress Tracking
- [x] XP, lessons, words, minutes counters
- [x] Weekly activity bar chart
- [x] Quiz performance history
- [x] Achievements gallery (6 achievements)
- [x] Level progression system

## AI Tutor Chat
- [x] Chat interface with AI tutor avatar
- [x] Backend LLM integration for personalized responses
- [x] Language-specific system prompt
- [x] Quick reply chips
- [x] AI personalized lesson recommendations

## Profile & Settings
- [x] User profile display (name, language, level)
- [x] Daily goal adjustment
- [x] Dark/light mode toggle
- [x] Language switching
- [x] Progress reset

## Navigation & Architecture
- [x] Bottom tab bar (Home, Lessons, Practice, Progress, Profile)
- [x] Stack navigators within tabs
- [x] Theme configuration (Indigo/Teal palette)
- [x] Icon mappings in icon-symbol.tsx
- [x] App branding (logo, splash, icon)

## Polish & Accessibility
- [x] Haptic feedback on key interactions
- [x] Smooth animations (card flips, quiz answer reveal)
- [x] All TypeScript errors resolved


## Authentication (NEW)
- [x] Registration screen (email, password, name, confirm password)
- [x] Login screen (email, password, remember me)
- [x] Form validation (email format, password strength, matching passwords)
- [x] Backend auth API integration (register, login, logout)
- [x] Session management and token storage
- [x] Auth state persistence across app restarts
- [x] Update root navigation to show auth flow before onboarding
- [x] Logout functionality in profile screen


## Quiz Enhancement
- [x] Expand quiz content to 10-20 questions per difficulty level
- [x] Create difficulty selection screen (Easy, Medium, Hard, Expert)
- [x] Update quiz data structure to include difficulty levels
- [x] Update quiz screen to filter questions by selected difficulty
- [x] Adjust XP rewards based on difficulty level (Easy: 50, Medium: 100, Hard: 150, Expert: 200)
- [x] Update quiz results to show difficulty-based scoring


## South African Language Migration
- [x] Update content data with 11 South African languages
- [x] Migrate lesson content to all SA languages
- [x] Migrate vocabulary data to all SA languages
- [x] Migrate quiz questions to all SA languages
- [x] Update onboarding language selection screen
- [x] Update language codes and metadata
- [x] Update documentation with SA language info
- [x] Test all language flows

## Certificate System
- [x] Add certificate tracking to user profile store
- [x] Create certificate data structure with ID, language, date, user name
- [x] Implement certificate generation logic when all lessons completed
- [x] Create certificate display screen with visual design
- [x] Add PDF export functionality for certificates
- [x] Add certificate display to progress/achievements screen
- [x] Add certificate sharing functionality (social media, email)
- [x] Test certificate generation and export
