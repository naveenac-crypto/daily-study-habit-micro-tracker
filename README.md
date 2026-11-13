# Daily Study & Habit Micro-Tracker

## Project Overview
DailyTrack is a browser-based dashboard for tracking daily habits,
study routines, focus sessions, and consecutive active days.

The main dashboard works without registration or login.
Records are stored locally in the browser.

## Course Details
- Course: Web Technology
- Course Code: 25CS208
- Assessment: IA-3 Microproject
- Academic Year: 2026–2027

## Student Details
- Name: Naveen Ac
- Register Number: URK26CS1224
- Batch: B4
- Faculty: DR. I Titus

## Live Website
https://daily-study-habit-micro-tracker.vercel.app

## GitHub Repository
https://github.com/naveenac-crypto/daily-study-habit-micro-tracker.git

## Main Features
- Create and edit recurring daily habits
- Mark habits completed for a selected day
- Archive habits while retaining earlier history
- View daily completion percentage and progress bar
- Use a Pomodoro timer with custom focus and break intervals
- Review completed focus sessions and daily focus minutes
- Track consecutive active days
- Save records using browser LocalStorage
- Export and restore JSON backups
- Switch between light and dark themes
- Use the responsive desktop and mobile dashboard
- Access an arithmetic calculator and study-time estimator
- Ask the keyword-based help chatbot about the application

## Technologies
- HTML5
- CSS3
- CSS Grid and Flexbox
- JavaScript
- LocalStorage
- GitHub
- Vercel

## Progress Calculation
Progress is the number of completed applicable habits divided by
the total applicable habits for the selected day, multiplied by 100
and rounded.

With no habits, progress is 0%.

## Streak Rule
A day is active when at least one habit or one full focus session
is completed.

The streak counts consecutive active local-calendar days through
today. If today is not active yet, it counts back from yesterday.
A missed day breaks the streak.

## Timer Behaviour
- Focus and break intervals can be customised.
- Pause preserves the remaining time.
- Reset discards the incomplete interval.
- Only completed focus intervals are recorded.
- Breaks do not count as study time.
- The next interval starts only when Start is pressed.
- Reloading resets an unfinished timer without recording completion.

## Assessment Form Demonstrations
Registration, sign-up, and sign-in pages demonstrate client-side
validation for the course assessment.

They do not create real accounts or save passwords.
The tracker itself does not require login.

Fictional demo sign-in:
- Email: demo@example.com
- Password: Demo@123

These are public demonstration credentials, not a real account.

## Run Locally
1. Download or clone this repository.
2. Open the folder containing index.html in VS Code.
3. Run index.html using Live Server.
4. Open the dashboard.

## Privacy and Limitations
- Habit records are stored in the browser, not an application database.
- Records are not encrypted or automatically synchronised.
- Clearing browser/site data may remove records.
- Export a JSON backup before clearing data.
- Hosting providers still receive normal website requests.
- The chatbot uses keyword matching, not a trained AI model.
- Use one active tracker tab to reduce conflicting changes.
- No bank connection, external AI service, or analytics script is included.

## Testing Status
JavaScript syntax and local HTML asset references were checked
during preparation.

Browser, device, persistence, backup, and timer tests must be
recorded in TEST-PLAN.csv. Only mark tests passed after observing
the results.

## Development Note
AI assistance was used to prepare the starter implementation
and documentation. The submitting student must review, adapt,
test, and explain the project and describe actual contributions.
