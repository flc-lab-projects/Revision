# Révisions

Three small revision apps for school, published as one static site. No build step,
no dependencies, no network calls beyond the site's own files. Everything works
offline once a page has loaded, and all progress is stored on the device.

    https://flc-lab-projects.github.io/Revision/

The landing page lists the three apps and shows how much has been done in each.

| Folder | App | What it covers |
|---|---|---|
| `allemand/` | Boîte à mots | German ↔ French vocabulary: flashcards and a typing exercise |
| `livrets/` | Les livrets | Times tables 1–12: practice pile and a 30-in-3-minutes test |
| `francais/` | Les phrases | Grammaire 7P: types and forms of sentences |

Each folder has its own README explaining how to add content to that app.

## Adding a new app

Create a folder, put an `index.html` and an `icon.png` in it, then add a block to the
`.apps` list in the root `index.html`. The tiles are plain links — there is no routing
or shared code between the apps, deliberately: one can break without touching the others.

## Notes

- The interface is in French throughout, since that's the language the learner already
  speaks. German and English appear only as the subject being studied.
- Progress lives in the browser's local storage, shared across all three apps because
  they sit on one domain. Clearing Safari's website data resets everything.
- `robots.txt` and a `noindex` tag ask search engines to stay away. The site is public
  to anyone with the link — it is simply not meant to be findable.
- Keep the content generic. Textbook examples are fine; real names, addresses and
  phone numbers would turn a harmless public repo into an identifying one.

## On an iPhone

Open a page in Safari, then Share → Add to Home Screen. It launches full screen with
its own icon. The landing page can be added as a single icon, or each app separately.
