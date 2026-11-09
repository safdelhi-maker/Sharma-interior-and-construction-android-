# Sharma Interior & Construction — Android-first prototype

## Included
- Mobile-first customer home and services
- Consultation / quotation enquiry form
- Indicative square-foot cost planner (sample rates only)
- Local demo business inbox with status updates and CSV export
- Editable WhatsApp contact setting
- PWA manifest, service worker and app icon

## Run the prototype
Open `index.html` in a browser. For install/offline PWA testing, host the folder on an HTTPS site or run a local web server. On Android Chrome, open the hosted site and choose **Install app** / **Add to Home screen**.

## Important prototype limitations
- Enquiries are stored in the browser's local storage on that device only. They do not reach the business owner or sync between phones.
- The business desk is a demo view, not protected by staff authentication.
- Cost rates are illustrative defaults, not market quotations. Confirm actual rates, taxes, materials and scope before using them with customers.
- The WhatsApp number must be entered by the business owner; no number is hard-coded.
- Do not collect real customer information in this demo until a secure backend, privacy notice, access controls, backups and deletion process are implemented.

## Recommended production architecture
1. Android app: Capacitor wrapper around this UI, or a native Android app.
2. Backend: authenticated API plus managed database (for example Firebase or Supabase).
3. Customer enquiries: server-side validation, spam protection, consent and privacy controls.
4. Business dashboard: owner/staff login, role-based access, enquiry assignment and audit trail.
5. Notifications: opt-in push notifications and/or email/WhatsApp integration.
6. Analytics and crash reporting with appropriate disclosure and consent.

## Google Play release checklist
- Create/verify a Google Play Console developer account and complete identity verification.
- Choose the final app name, package ID, icon, screenshots and feature graphic.
- Publish a public privacy policy URL and complete the Data safety form accurately.
- Complete the target audience, content rating, app access and ads declarations.
- Build and test a signed Android App Bundle (`.aab`) on physical devices.
- Complete internal testing and any testing requirements shown in Play Console for the account.
- Submit the release for Google Play review.

This ZIP is a web prototype source package, **not** a signed APK or Play Store upload. Store publishing requires a production build, developer account access, policy declarations and review.
