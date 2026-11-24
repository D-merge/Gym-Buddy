# Gym Buddy

A companion app for class training. Everything is stored on the phone (localStorage). There's no back end.

## Program (fixed)
- Six-week blocks, repeating: weeks 1–2 at 10 reps, weeks 3–4 at 6 reps, weeks 5–6 at 3 reps.
- The week of Monday 23 November 2026 is week 3 (the first 6-rep week): Squat Mon, Bench Tue, Boxing Wed, Deadlift Thu, Shoulders Fri.
- Mon/Tue squat and bench swap each week, and Thu/Fri deadlift and shoulder press swap each week. Wednesday is always boxing.
- The block anchor is `settings.start` ('2026-11-09', the Monday of week 1).

The schedule logic is the `plan()` function in `index.html`.

## Deploy to GitHub Pages
1. Create a repo (e.g. `gym-buddy`) and push these files to the root of `main`.
2. Repo → Settings → Pages → Source: "Deploy from a branch", Branch: `main` / root.
3. The site will be at `https://<user>.github.io/gym-buddy/`.

## Install on a phone
- iPhone: open the link in Safari → Share → Add to Home Screen.
- Android: open in Chrome → Install app (or menu → Add to Home screen).

Install before logging. A home screen app on iPhone keeps its own storage, separate from Safari.
Deleting the app deletes its data, so use Me → Copy backup now and then.

## Updating
Change `VERSION` in `sw.js` whenever you push an update. Phones pick it up the next time they open the app with signal.
