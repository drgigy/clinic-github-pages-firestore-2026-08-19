# Clinic GitHub Pages Firestore Site

Static GitHub Pages copy of the clinic site.

## Deployment notes

- `CNAME` files from the source archive were intentionally omitted so this repo does not claim the existing `clinic.woyz.in` custom domain.
- `firestore.rules` contains the Firestore security rules for the new Firebase project.
- `firebase.json` points Firebase CLI deployments at `firestore.rules`.
- Firestore data is scoped per signed-in user under `users/{uid}/...`.
- After a new Firebase project is created, update the Firebase web app config in the HTML files before publishing.
