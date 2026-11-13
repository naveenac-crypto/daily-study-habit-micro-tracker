# DailyTrack — Daily Study & Habit Micro-Tracker
25CS208 Web Technology | IA-3 | Student name/register number: TO COMPLETE

## Start here
1. Extract this package into a normal folder.
2. Open the website folder in VS Code. Use Live Server to open index.html.
3. Choose Open dashboard — no login. Use fictional demonstration information.
4. Add three habits; tick one. Expected progress: 33%. Tick all: 100%.
5. For a quick real timer demonstration choose focus 1 minute and break 1 minute, Apply, Start, and wait for completion. One full focus session is logged; a break never counts as study time. Never shorten a countdown secretly and describe it as a full session.
6. Keep the same browser/profile/origin for persistence. Export JSON before clearing data.

## Assessment forms
Registration and sign-up are OPTIONAL VALIDATION DEMOS: they do not create accounts or save passwords. Dashboard requires no login. This deliberate boundary preserves the topic's no-login requirement but may require faculty confirmation for FR-03's account-creation wording. Do not represent these forms as real authentication.
Demo signin: demo@example.com / Demo@123.
Test registration: Student Demo / URK26CS001 / student@example.com / 9876543210 / CSE / Demo@123 (twice).

## Features and definitions
Habits repeat from their local-calendar creation day. Past-day entry is allowed; future checklist dates are not. Edit changes the habit label globally. Archive ends the habit from the selected day; earlier history stays, while later completions for that habit are removed after confirmation.
Progress: completed applicable habits / all applicable habits × 100, rounded. With no habits: 0%.
Active day: at least one checked habit OR completed focus session. Streak counts consecutive active calendar days through today, or through yesterday when today is not active. It resets after a missed day. This is not an all-habits-completed streak. Unchecking or archiving can change history and streak. No fabricated history is preloaded.
Timer: custom work 1–180 and break 1–60 whole minutes. setInterval refreshes a timestamp-derived remaining value. Pause retains remaining time; reset discards partial time. No automatic next-phase start. Completed work logs for the local day when completion is detected, even if the tab was delayed across midnight. Reload abandons the timer, not stored habits/session history. Timer state is NOT persisted. A best-effort tab ownership lock reduces duplicate timers but does not provide atomic cross-tab concurrency. Use one active tracker tab, especially when editing or importing.

## Privacy boundaries
This code makes no application API/analytics calls. Static hosting still receives ordinary requests. Local records are NOT encrypted, NOT protected by accounts, NOT cloud-backed, and can be read by others using the browser profile. Browser or device time changes affect dates, streaks and deadlines. No notification permission, sound alarm or offline install/service worker is included. Offline access from the deployed site is not guaranteed.

## Verification status
JavaScript syntax checked using node --check. HTML unique IDs and referenced local asset inclusion checked. No interactive browser, physical-device, accessibility or deployment tests have been performed here. TEST-PLAN.csv starts NOT RUN. Test before submitting. Do not claim industry security or a 100% checklist pass.

## GitHub + Vercel
Create a NEW repository for this friend/project. Upload all website files individually, with index.html at repository root. Include README; exclude personal backups, secrets and signed documents. Use genuine commit messages. Do not reuse the expense-tracker repository or links.
Import that repository into a new Vercel project as a static/Other project, no build command. Verify the actual assigned URL and all five .html pages. If using drag/drop, upload the extracted website files, not an extra wrapping folder.
Replace LIVE_URL and REPO_URL in your documents only after creation. No deployment or repository is created by this package.
QR codes require the actual final URLs. Scan both before recording.

## Files
index/register/signup/signin/home.html: five pages.
styles.css/layout.css: shared visual system and Grid/Flexbox.
app.js: habits, calendar records, progress, streak and backups.
timer.js: Pomodoro and completed-session logging.
validation.js/theme.js/calculator.js/chatbot.js: assessment modules.

## Academic use
AI-assisted starter. Student must review, adapt, test, explain actual contributions and follow institutional AI policy. Do not claim unaided authorship, fabricated tests, fake history or signatures.
