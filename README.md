# Favicon Generator

Make a favicon from text, an emoji, or an uploaded image, right in your browser.

**Live demo:** https://0xelitesystem.github.io/favicon-generator/

## Use

1. Open the tool and pick a source: **Text / Emoji** or **Image**.
2. For text, type a letter, a couple of characters, or a single emoji, then choose a font, weight, and text color. For an image, select a file and choose cover or contain fit.
3. Set the background color (or make it transparent), pick a shape (rounded, square, or circle), and adjust padding.
4. Watch the live preview render at 16, 32, and 48 px, the exact sizes browsers use.
5. Download the files you need:
   - **favicon.ico**, a single multi-resolution file bundling the 16, 32, and 48 px images.
   - **PNG** at 16, 32, 48, 180 (Apple touch icon), 192, and 512 px.
6. Copy the ready-made `<link>` tags and paste them into your page `<head>`.

Empty or invalid input is caught and reported before you can export, so you never save a blank file.

## Why this exists

Most favicon makers upload your artwork to a server, wrap the result in an account wall, or bury it under ads and trackers. This one does the whole job locally. It is a single HTML file with no framework, no fonts, no analytics, and no network calls, so there is nothing to phone home. The `.ico` writer is a real ICO encoder, not a renamed PNG, so the file works the way browsers expect. MIT licensed, so you can read every line, fork it, or self-host it.

## Privacy

Everything runs in your browser. Your text and any image you choose are processed on your own machine using the Canvas API and never leave it. There is no upload, no server, no cookie, and no request of any kind. You can confirm this by opening the tool with your network disconnected, or by watching the network tab stay empty.

## Run locally

Clone the repo and open the file, or serve it with any static server:

```
git clone https://github.com/0xelitesystem/favicon-generator.git
cd favicon-generator
# either open index.html directly in a browser, or:
python -m http.server
# then visit http://localhost:8000
```

## Build

There is no build step. The tool is one self-contained `index.html` with inline CSS and JavaScript. Nothing to install, nothing to compile.

## More

Part of a catalog of single-file browser tools and plain-language references, all MIT licensed and dependency-free: [0xelitesystem.github.io](https://0xelitesystem.github.io/). Built by [elitesystem.ai](https://elitesystem.ai).

## License

MIT. See [LICENSE](LICENSE).

## Related

- https://github.com/0xelitesystem/jwt-inspector
- https://github.com/0xelitesystem/eeat-signals-reference
