# Mellow Box

The Crossroad Digger record collection: CDs, LPs, music films and books.

This site is generated; edit the source data, not index.html.

### Japanese (added by hand, outside the generator)

Japanese (日本語) lives in `i18n/ja.js`, not in the generated `I18N` table, so it survives a rebuild. When regenerating `index.html`, keep these two things or Japanese disappears:

1. `<script src="i18n/ja.js"></script>` just before the main `<script>` that defines `LANGS`.
2. The `MB_EXTRA` hook line right after `const I18N={...};`, which adds each extra language to `LANGS`, `LOC` and `I18N`.

`i18n/ja.js` is keyed by the French source text, like `I18N`. When a new interface text is added, add its Japanese there too (untranslated texts fall back to English). Album notes (`r`, `n`) have no Japanese version, like the other non-French languages: they show the English `r_en` / `n_en`.

## Portastudio 424

`portastudio/` is hand-written (not generated): a guide to the TASCAM Portastudio 424 MKIII, served at https://crossroaddigger.github.io/portastudio/.

- `portastudio/index.html` holds the layout, styles and app logic.
- `portastudio/lang/{en,fr,nl,de,es,it,pt}.js` hold all the text, one file per language, same structure in each. Edit text there.
- The language comes from `?lang=xx`, then the `mb-lang` choice shared with the Mellow Box homepage, then the browser language, then English.
- `portastudio/424mkiii.jpg` / `.webp` is the illustration, re-encoded with all metadata removed.

## Web MiniDisc

`minidisc/` is hand-written (not generated) and deliberately separate from Mellow Box: its own look, title, icon and texts, no link to or from the Mellow Box pages, no shared language setting. The visit counter is the same GoatCounter account (mellowbox.goatcounter.com), with its pages under `/minidisc/`. Served at https://crossroaddigger.github.io/minidisc/.

- `minidisc/index.html` is the whole page, in 8 languages (fr, en, nl, de, es, it, pt, ja): texts are in the `T` object at the bottom. The language comes from `?lang=xx`, then its own `wmd-lang` choice (not shared with Mellow Box), then the browser language, then English. It presents Web MiniDisc Pro (https://web.minidisc.wiki/, by asivery, based on Stefano Brilli's Web MiniDisc); the only thing it shares with Mellow Box is the Buy Me a Coffee link (buymeacoffee.com/mellowbox).
