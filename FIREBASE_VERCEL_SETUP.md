# Firebase + Vercel Setup

The production Firebase project configured in this build is:

- Project ID: `inventorymanagement-syst-63945`
- Auth domain: `inventorymanagement-syst-63945.firebaseapp.com`
- Vercel domain: `inventorymanagement-system-beta.vercel.app`

## Required Firebase Console settings

### 1. Authorized domain

Open Firebase Console -> Authentication -> Settings -> Authorized domains and add:

`inventorymanagement-system-beta.vercel.app`

Do not include `https://` or a trailing `/`.

### 2. Google provider

Open Firebase Console -> Authentication -> Sign-in method and make sure **Google** is enabled.

### 3. Redeploy

After saving the Firebase settings, redeploy the project on Vercel or wait for the next deployment, then open:

`https://inventorymanagement-system-beta.vercel.app/`

## Important

The client-side Firebase API key is intended to be present in web application code. Access control is enforced by Firebase Authentication and Firestore Security Rules.

This build uses the default Firestore database of `inventorymanagement-syst-63945`. If your existing business data is stored in a different Firebase project or a named Firestore database, do not switch projects/databases without migrating or intentionally reconnecting that data.
