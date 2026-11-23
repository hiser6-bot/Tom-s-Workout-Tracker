# Tom's Workout Tracker - Original Integrated Build

This build starts with the recovered original `index.html` and preserves the original day tabs, embedded exercise photos, sets/reps/weight tracking, session checks, charts, history, backup export, dark mode, install support, and rest timers. It adds **+ Add Workout** for strength, elliptical, treadmill, rowing, bike, mobility, and other activities.

## Install to GitHub Pages
1. Download a backup of the current repository.
2. Upload all files in this package to the repository root.
3. Commit the files.
4. Wait 1-3 minutes for GitHub Pages deployment.
5. On the phone, fully close and reopen the installed app. If the old version remains, clear the site cache or remove and re-add the home-screen app.

## Data compatibility
The original keys remain unchanged: `workoutDraft`, `workoutHistory`, `currentDay`, and `darkMode`. Added workouts use separate keys: `addedWorkouts`, `addedWorkoutDraft`, and `addedWorkoutTemplates`. Export Data now includes both original and added workout records.
