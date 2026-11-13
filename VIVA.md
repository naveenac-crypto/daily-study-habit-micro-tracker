# Quick viva
What is the project? A no-login browser-local habit checklist, focus timer and activity streak dashboard.
Progress formula? Checked applicable habits divided by all applicable habits, times 100, rounded; zero habits means zero percent.
Active day? At least one completed habit or full focus session.
Streak? Consecutive active local-calendar days ending today, or yesterday if today is not active yet. Missed day breaks it.
How persist? JSON.stringify to LocalStorage; JSON.parse and schema validation when loading.
Timer? setInterval updates presentation, but remaining time comes from deadline minus Date.now(). clearInterval stops updates. Reload resets it; completion is logged when detected.
Why not subtract one each second? Delayed callbacks in background tabs would cause drift; a deadline reduces that error but clock changes still affect it.
Privacy? No application analytics/API calls, but hosting still gets requests. LocalStorage is not encrypted and does not isolate people sharing a browser profile.
Login? Optional assessment UI only, not real authentication. Dashboard has no login dependency.
Backup? Export JSON; restore validates schema before replacing data after confirmation.
Archive? Ends a habit from selected date and removes later completions, preserves older history.
Concurrency? Best-effort timer ownership, not atomic locking; use one tab.
Future scope? Safer recovery, accessible notifications, offline installation, broader tests; never claim these exist now.
GitHub vs Vercel? Source/change history vs live hosting.
Your work? Explain only actual contributions and disclose assistance under faculty rules.
