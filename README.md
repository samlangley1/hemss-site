# hemss public website

Static homepage and privacy policy for hemss, the Google OAuth app name used by the Dmiko / yt-slower local YouTube automation project. No build, backend, dependencies, forms, or tracking scripts.

## Enable GitHub Pages

1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Choose branch **main**, folder **/(root)**, and click **Save**.
4. Wait for the Pages deployment to complete. Confirm both links below load publicly before using them in Google Cloud.

Homepage: https://samlangley1.github.io/hemss-site/

Privacy policy: https://samlangley1.github.io/hemss-site/privacy.html

In Google Cloud → Google Auth Platform → Branding, enter these in **Application home page** and **Application privacy policy link**, then save. Keep the app name consistent with hemss. Publishing status and any verification requirements are managed separately in Google Cloud; this website does not guarantee approval.

## Files

- `index.html`: app purpose, workflow, authorization explanation, support.
- `privacy.html`: data access, purpose, storage, external services, retention, revocation, deletion, and website hosting.
- `styles.css`: responsive shared design using system fonts.
- `.nojekyll`: serve the files directly.

Edit HTML/CSS and push to main to update the site after Pages is enabled. Preview locally with `python -m http.server 8000` and visit http://localhost:8000.

Only public website content belongs here. Never add OAuth client credentials, API keys, refresh tokens, application databases, logs, or media. Update the privacy policy whenever actual application data practices change.
