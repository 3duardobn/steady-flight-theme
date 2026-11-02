# Steady Flight — theme for Firefox-based browsers

Port of the **Steady Flight** theme (Chrome Web Store) to any Firefox-based
browser — Firefox, Zen, Waterfox, Floorp and others — plus a matching
**Sidebery** theme.

It uses `userChrome.css` and `userContent.css`, so there is no extension and
no signed theme to install.

![Steady Flight](browser/chrome/steady-flight/ntp.png)

- Original theme: **Steady Flight** by **Shyama Kuver** — [heartovercrown.com](https://www.heartovercrown.com/)
- Chrome Web Store: [chromewebstore.google.com/detail/steady-flight](https://chromewebstore.google.com/detail/steady-flight/bngmkpbgamlgojclkfkbpmikjilmkdfp)

## Colors

| Use | Hex |
| --- | --- |
| Frame / panel | `#465f4e` |
| Toolbar / active tab | `#5b7763` |
| New tab background | `#809e88` |
| Accent (terracotta) | `#d76435` |
| Taupe from the artwork | `#9e8369` |
| Text | `#ffffff` |

## Files

```text
browser/chrome/
├── userChrome.css              # imports the browser theme
├── userContent.css             # imports the new tab theme
└── steady-flight/
    ├── steady-flight.css       # tabs, toolbars, menus, sidebar
    ├── newtab.css              # new tab layout
    ├── ntp-data.css            # artwork embedded as a data: URL
    └── ntp.png                 # original 1366×768 artwork
sidebery/
└── steady-flight-sidebery.css  # Sidebery theme
```

## Install

1. Copy the contents of `browser/chrome/` into your profile's `chrome/` folder
   (`about:profiles` shows the path).
2. In `about:config`, set
   `toolkit.legacyUserProfileCustomizations.stylesheets = true`.
3. Close **all** browser windows and open the browser again — `userChrome.css`
   is only read at startup.

Sidebery: open **Settings → Styles → Styles editor**, paste
`sidebery/steady-flight-sidebery.css` and save.

## License

The **code** (CSS, HTML and scripts in this repository) is in the **public
domain**, under the [Unlicense](LICENSE).

The **artwork and visual identity** of the original theme belong to **Shyama
Kuver** and are used here for personal use only, with credit. See
[NOTICE.md](NOTICE.md).
