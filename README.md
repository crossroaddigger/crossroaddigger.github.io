# Mellow Box

The Crossroad Digger record collection: CDs, LPs, music films and books.

This site is generated; edit the source data, not index.html.

## Portastudio 424

`portastudio/` is hand-written (not generated): a guide to the TASCAM Portastudio 424 MKIII, served at https://crossroaddigger.github.io/portastudio/.

- `portastudio/index.html` holds the layout, styles and app logic.
- `portastudio/lang/{en,fr,nl,de,es,it,pt}.js` hold all the text, one file per language, same structure in each. Edit text there.
- The language comes from `?lang=xx`, then the `mb-lang` choice shared with the Mellow Box homepage, then the browser language, then English.
- `portastudio/424mkiii.jpg` / `.webp` is the illustration, re-encoded with all metadata removed.

## Web MiniDisc

`minidisc/` is hand-written (not generated) and deliberately separate from Mellow Box: its own look, title, icon and texts, no link to or from the Mellow Box pages, no shared language setting or analytics. Served at https://crossroaddigger.github.io/minidisc/.

- `minidisc/index.html` is the whole page (French). It presents Web MiniDisc Pro (https://web.minidisc.wiki/, by asivery, based on Stefano Brilli's Web MiniDisc); the only thing it shares with Mellow Box is the Buy Me a Coffee link (buymeacoffee.com/mellowbox).
