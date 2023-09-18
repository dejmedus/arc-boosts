## Arc Browser Boosts ⭐

Snippets to 'boost' websites on [Arc browser](https://arc.net/)

### How to add a boost

1. Go to target website
2. cmd+t "new boost"
3. Click Code
4. Copy in the boost to CSS tab

---

### All Boosts

- [Centered Linux Manual](#linux-manual)
- [Gray-scale Pygame Docs](#pygame-docs)
- [No Dev.to Sidebars](#devto)
- [Simple TikTok](#tiktok)

---

### Linux Manual

Changes the text colors to gray-scale and centers the linux manual pages

#### URL: https://man7.org/linux/man-pages

<img width="1792" alt="Linux manual webpage" src="https://github.com/dejmedus/arc-boosts/assets/59973863/bcf5014c-d77b-4cfb-af06-5630419979e4">

```css
:root {
  --text: black;
  --bg: white;
  --grey: rgb(78, 78, 78) !important;
  --primary: rgb(56, 125, 255) !important;
  --primary-hover: rgba(56, 126, 255, 0.25) !important;
}

@media (prefers-color-scheme: dark) {
  :root {
    --text: white;
    --bg: black;
    --grey: rgb(189, 189, 189) !important;
    --primary: rgb(106, 158, 255) !important;
    --primary-hover: rgba(162, 195, 255, 0.25) !important;
  }
}
* {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif !important;
}
html {
  background-color: var(--bg) !important;
}
body {
  color: var(--text) !important;
  background-color: var(--bg) !important;
  display: grid;
  align-items: center;
  justify-content: center;
  width: 100vw;
  font-size: 110% !important;
}
.nav-bar {
  background-color: var(--bg) !important;
  margin-top: 0.4em;
}
.nav-end {
  opacity: 0;
}
.man-search input {
  min-width: 200px;
  padding: 0.28em;
}

h1,
h2,
b {
  color: var(--text) !important;
}
pre,
i {
  color: var(--grey) !important;
}
strong {
  color: var(--grey) !important;
}
a {
  color: var(--primary) !important;
}
a img {
  display: none;
}
a:hover,
a:active,
a:focus {
  background-color: var(--primary-hover) !important;
}
.footer {
  background-color: var(--bg) !important;
}
```

### Pygame Docs

Changes the pygame docs color pallette from greens to gray-scale

#### URL: https://www.pygame.org/docs/

<img width="1272" alt="pygame docs" src="https://github.com/dejmedus/arc-boosts/assets/59973863/5b576734-fc18-4092-9d7a-7659c1a6d708">

```css
.document {
  background-color: white !important;
}

/* footer*/
.related {
  background-color: rgb(245, 245, 245) !important;
  border: 0 !important;
}

/* header and code block highlight */
pre,
.header .logo,
.header .flex-container {
  background-color: rgb(245, 245, 245) !important;
}

/* links */
.reference.internal em {
  background-color: #cae8ff !important;
}

/* button color */
.addcomment input,
a.commentButton {
  background-color: black !important;
  color: white !important;
}
```

### Dev.to

Removes the Dev.to sidebars

#### URL: https://dev.to

<img width="1274" alt="devto" src="https://github.com/dejmedus/arc-boosts/assets/59973863/d62f902e-40f1-433c-ba84-5a9faa6188aa">

```css
#sidebar-wrapper-left {
  visibility: hidden;
  width: 5px !important;
}

#sidebar-wrapper-right {
  visibility: hidden;
  width: 5px !important;
}
```

### TikTok

Removes sidebar info and lowers icon opacity unless hovered

#### URL: https://tiktok.com

<img width="1787" alt="simple-tiktok" src="https://github.com/dejmedus/arc-boosts/assets/59973863/2888d640-a847-4b44-84cb-8a7f9225a589">

```css
[class*="DivUserContainer"] {
  visibility: hidden;
}
[class*="DivFooterContainer"] {
  visibility: hidden;
}
[class*="DivMessageIconContainer"] {
  visibility: hidden;
}
[class*="DivHeaderLeftContainer"] {
  visibility: hidden;
}
[class*="DivUpload"] {
  visibility: hidden;
}
[class*="DivHeaderInboxContainer"] {
  visibility: hidden;
}
[class*="AppText"] {
  visibility: hidden;
}
/* music icon */
/* [class*="StyledIcon"] {
  visibility: hidden;
}
[class*="MusicText"] {
  visibility: hidden;
} */
[class*="StyledFollowButtonTux"] {
  opacity: 40%;
}
[class*="StyledFollowButtonTux"]:hover {
  opacity: 100%;
}
[class*="SpanIconWrapper"] ~ strong {
  visibility: hidden;
}
[class*="SpanIconWrapper"]:hover ~ strong {
  visibility: visible;
}
[class*="SpanIconWrapper"] {
  opacity: 40%;
}
[class*="SpanIconWrapper"]:hover {
  opacity: 100%;
}
[class*="UlMainNav"] {
  opacity: 40%;
}
[class*="UlMainNav"]:hover {
  opacity: 100%;
}
```
