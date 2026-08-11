# The two pages Apple asks for

App Store Connect will not take a submission without a **support URL** and a
**privacy policy URL**. These are those two pages, and nothing else: no build
step, no framework, no tracking — the same paper, plum and river colours the app
itself wears, and the same two typefaces, served from this folder.

    index.html      Support — how to open a file, how to move to a new phone,
                    what to do when a relationship comes out wrong
    privacy.html    Privacy — what the app holds, what leaves the phone, and
                    the three permissions it asks for
    style.css       both pages
    fonts/          Fraunces and Space Mono, copied from app/web/fonts

## Before you publish

Both pages carry `you@example.com` twice — in the `mailto:` and in the visible
text. Search for it and put your own address in; an address that bounces is a
rejected submission.

## Putting it on GitHub Pages

Make a repository — `riverkin-support` does the job — and push the contents of
this folder to its root, so that `index.html` is the top of the repository. Then
**Settings → Pages → Deploy from a branch → main → / (root)**.

A minute later the two URLs App Store Connect wants are:

    https://<your-github-name>.github.io/riverkin-support/
    https://<your-github-name>.github.io/riverkin-support/privacy.html

If you would rather keep the site inside a repository that already holds the
app, put these files in a `docs/` folder at the repository root and choose
**/docs** instead of **/ (root)** on that same settings page.

## When the app changes

The privacy page says what version it describes and when it came into force.
If a later version ever does something the page does not describe — anything
that reaches the network, for one — rewrite the page first and move the date.
