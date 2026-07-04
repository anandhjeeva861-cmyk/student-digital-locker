# TODO - Student Locker Frontend Updates

## Step 1: Remove notification section for students ✅
- Edit `assets/js/layout.js`
  - For student role: hide navbar bell icon (done).
  - Notifications sidebar item is removed by removing Notifications from `STUDENT_MENU` (done).

## Step 2: Personal details first-time completion flow ✅
- Edit `assets/js/login.js`
  - On successful registration: save personal details into `sl_profile` and mark `sl_profile_completed=true`.
  - Prevent duplicates by overwriting `sl_profile` (done).

## Step 3: Profile page read-only after completion ✅
- Edit `profile.html`
  - If `sl_profile_completed` is true: hide edit form and show read-only view + “Edit Profile”.
  - Edit mode re-enables the form and keeps validation.

## Step 4: Hide/disable “Complete Personal Details” navigation ✅
- Edit `assets/js/layout.js`
  - If incomplete: show “Complete Personal Details” CTA (as a sidebar link to profile.html).
  - If complete: show normal Profile menu only.

## Step 5: Quick verification
- Manual checks (recommended):
  - Register as a student: verify `sl_profile` saved and profile edit form not shown after completion.
  - Login as student: verify Personal Details read-only.
  - Teacher screens unchanged.
  - Student navbar/bell + sidebar Notifications link are gone.


