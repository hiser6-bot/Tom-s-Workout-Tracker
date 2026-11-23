# Tom's Workout Planner 365: Add Workout

A mobile-first, installable workout-entry screen for GitHub Pages. It supports strength, elliptical, treadmill, rowing, bike, mobility, and other ad hoc workouts. Added workouts are stored locally in the browser and tracked with the same detail as planned workouts.

## Features
- Exercise-by-exercise weight, set, rep, and completion tracking
- Cardio-specific fields for elliptical, treadmill, rowing, and bike
- RPE, total time, notes, and shoulder/elbow pain tracking
- Draft saving and reusable workout templates
- Multiple workouts per date
- JSON export
- Offline-capable Progressive Web App
- Light and dark mode

## Publish with GitHub Pages
1. Create a new GitHub repository, for example `toms-workout-planner-365`.
2. Upload every file from this folder to the repository root.
3. In GitHub, open **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select **main** and **/(root)**, then click **Save**.
6. After GitHub finishes publishing, open the Pages URL shown in Settings.

## Add to an existing planner
Copy `index.html`, `styles.css`, and `app.js` into the existing project, or move this screen into an `add-workout/` folder. The localStorage keys are:

- `tomsWorkoutPlanner365.workouts.v1`
- `tomsWorkoutPlanner365.draft.v1`
- `tomsWorkoutPlanner365.templates.v1`

The saved workout object uses `source: "added"`, so scheduled and ad hoc workouts can share the same reporting pipeline while remaining distinguishable.

## Important data note
This version stores data in the browser on the current device. Clearing browser/site data removes it. Use **Export JSON** for backups. To sync across devices, connect the save/load functions to a backend such as Supabase or Firebase.
