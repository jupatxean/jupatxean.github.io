# jupatxean.github.io

The public site for **JupaFit**. Two pages, no build step, no JavaScript.

| File | What it is |
| --- | --- |
| `index.html` | A landing page, mostly so the root is not a 404 |
| `privacy.html` | The privacy policy, required by both app stores |

## privacy.html is generated

Do not edit it here. The words live in the app repository, at
`docs/PRIVACY_POLICY.md`, and `tools/build_privacy_page.py` renders this file
from them. Editing this copy produces two versions of a legal document that
disagree, with no way to tell which one a user read.

To publish a change: edit the markdown in the app repo, re-run the script,
copy `site/privacy.html` over this file, commit, push.
