# vc-CSS-Snippets

A compilation of CSS snippets for Discord and its custom clients.

## About

This repository is a collection of various CSS snippets that I have gathered for personal use to enhance and
customize the appearance of Discord and its custom clients. The primary purpose of this repository is to serve as a
personal reference.

Please note that the original authorship of some code snippets may belong to other developers, and I have posted
them here for convenience.

## Disclaimer

Discord is a trademark of Discord Inc. and is solely mentioned for the sake of descriptivity. Mention of it does not
imply any affiliation with or endorsement by Discord Inc.

## Installation

1. Open Vencord settings, then **Themes**, then **Edit QuickCSS**.
1. Paste the imports below at the top of QuickCSS and save.
1. Remove the lines of any snippet you do not want. Keep the order: `accent.css` and `glow.css` must load after
   `midnight-catppuccin-mocha.css`, because they override its colors.

```css
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/midnight-catppuccin-mocha.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/server-columns.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/better-message-buttons.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/pretendard.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/full-height-picker.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/hide-quests.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/dual-line-chatbox.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/colored-role-pills.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/compact-dm-buttons.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/bubble-usernames.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/timestamp-bubbles.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/better-quotes.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/accent.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/glow.css");
@import url("https://raw.githubusercontent.com/slopization/vc-CSS-Snippets/refs/heads/main/Snippets/gradient-status.css");
```

The links use the `refs/heads/main` form; the shorter `main/` form did not load in Vencord.

To change the number of server columns, add this below the imports:

```css
:root body {
  --server-columns: 3;
  --server-column-gap: 12px;
}
```

## Loading a new version

GitHub serves these files with a five minute cache, and Discord keeps its copy even across `Ctrl+R`. To load the
latest version right after it is pushed:

1. Press `Ctrl+Shift+I` to open DevTools.
1. In the **Network** tab, check **Disable cache**.
1. Keep DevTools open and press `Ctrl+R`.

## Class updates

Discord renames its CSS classes with most updates. The **Update Classes** workflow in the Actions tab replaces every
renamed class it can map to a single new name, commits the result, and lists the rest in its run summary.

## Usage

Feel free to use any of the snippets provided in this repository. However, be aware that you do so at your own risk.
I do not take any responsibility for issues that may arise from the use of these snippets.

## Contributions

Since this is a personal project, contributions are not expected. However, if you have suggestions or improvements,
feel free to open an issue or a pull request.

## License

This repository is not licensed for distribution, and the snippets are shared for personal use only.
