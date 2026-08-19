# Clinic GitHub Pages Site

Static GitHub Pages copy of the clinic site.

## Deployment notes

- `CNAME` files from the source archive were intentionally omitted so this repo does not claim the existing `clinic.woyz.in` custom domain.
- `firestore.rules` contains the cloud data security rules.
- `firebase.json` points CLI deployments at `firestore.rules`.
- Cloud data is scoped per signed-in user under `users/{uid}/...`.
- The web app config points to the reused `woyz-check-in` project.
