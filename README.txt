ROSE WRENCH FIREBASE RESET PAGE

Open reset.html in a browser.

This page uses the same Firebase project/config as the Rose Wrench scheduler and the supplied Firebase example page.

It deletes:
- scheduler/settings
- all scheduler/services documents
- all scheduler/bookings documents

Then it recreates:
- Monday-Friday: 08:00-17:00
- Saturday: 09:00-14:00
- Sunday: closed
- Oil Change: 45 minutes
- Brake Service: 120 minutes
- Diagnostic: 60 minutes
- General Repair: 180 minutes

It does NOT delete products_bracelets.

IMPORTANT:
Firebase Firestore Security Rules must allow the browser to perform these operations. For a production site, do not leave unrestricted public write/delete access enabled; protect the owner/reset functions with Firebase Authentication and rules.
