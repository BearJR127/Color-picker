# Color Picker

This simple web app uses Firebase Realtime Database to coordinate sender/receiver sessions.

## Firebase Setup

1. Create a Firebase project and Realtime Database.
2. Copy your project's configuration into `index.html` and `dashboard.html`.
3. Deploy the database rules from `firebase-rules.json`:

```bash
firebase deploy --only database
```

If the rules are not deployed, writes may fail with `permission_denied` errors even if `firebase-rules.json` allows access.

Ensure the `databaseURL` in the HTML matches your Firebase project's database URL and that your hosting domain is added to Firebase's authorized domains.
