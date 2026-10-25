# jupatxean.github.io

The public site for **JupaFit**. A few pages, no build step.

| File | What it is |
| --- | --- |
| `index.html` | A landing page, mostly so the root is not a 404 |
| `privacy.html` | The privacy policy, required by both app stores |
| `terms.html` | The terms of use. Apple requires a link on the paywall |
| `duo/index.html` | Duo invite links (`/duo/?c=A1B2C3D4`). With the app installed iOS opens the app instead; without it this page shows the code and the App Store link |
| `.well-known/apple-app-site-association` | Tells iOS that `/duo/*` links belong to the app (universal links). Team SFPWYKMJH5 |
| `.nojekyll` | Empty. Without it GitHub Pages skips `.well-known/` |

## privacy.html and terms.html are generated

Do not edit it here. The words live in the app repository, at
`docs/PRIVACY_POLICY.md` and `docs/TERMS_OF_USE.md`, and
`tools/build_legal_pages.py` renders these files from them. Editing this copy produces two versions of a legal document that
disagree, with no way to tell which one a user read.

To publish a change: edit the markdown in the app repo, re-run the script,
copy `site/privacy.html` and `site/terms.html` over, commit, push.
