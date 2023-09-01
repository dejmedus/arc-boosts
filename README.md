## Arc Browser Boosts ⭐

Snippets to 'boost' websites on [Arc browser](https://arc.net/)

### How to add a boost

1. Go to target website
2. cmd+t "new boost"
3. Click Code
4. Copy in the boost to CSS tab

----

### All Boosts

- [Grayscale Pygame Docs](#grayscale-pygame-docs)
- [No Dev.to Sidebars](#simple-devto)
- [Simple TikTok](#simple-tiktok) 

----

### Grayscale Pygame Docs

Changes the pygame docs color pallette from greens to grayscale

| Template | URL                          |
| -------- | ---------------------------- |
| Style    | https://www.pygame.org/docs/ |


<details>
<summary>View</summary>
    
<img width="1272" alt="pygame docs" src="https://github.com/dejmedus/arc-boosts/assets/59973863/5b576734-fc18-4092-9d7a-7659c1a6d708">

</details>

```css
.document{
    background-color: white !important;
}

/* footer*/
.related{
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
.addcomment input, a.commentButton {
background-color: black !important;
color: white !important;
}
```

### Simple Dev.to

Removes the Dev.to sidebars

| Template | URL            |
| -------- | -------------- |
| Style    | https://dev.to |

<details>
<summary>View</summary>
    
<img width="1274" alt="devto" src="https://github.com/dejmedus/arc-boosts/assets/59973863/d62f902e-40f1-433c-ba84-5a9faa6188aa">

</details>

```css
#sidebar-wrapper-left{
  visibility: hidden;
  width: 5px !important;
}

#sidebar-wrapper-right{
  visibility: hidden;
  width: 5px !important;
}
```

### Simple TikTok

Removes sidebar info and lowers icon opacity unless hovered

| Template | URL                |
| -------- | ------------------ |
| Style    | https://tiktok.com |

<details>
<summary>View</summary>
    <img width="1787" alt="simple-tiktok" src="https://github.com/dejmedus/arc-boosts/assets/59973863/2888d640-a847-4b44-84cb-8a7f9225a589">
</details>

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
[class*="SpanIconWrapper"] ~ strong{
  visibility: hidden;
}
[class*="SpanIconWrapper"]:hover ~ strong{
  visibility: visible;
}
[class*="SpanIconWrapper"]{
  opacity: 40%;
}
[class*="SpanIconWrapper"]:hover{
  opacity: 100%;
}
[class*="UlMainNav"]{
  opacity: 40%;
}
[class*="UlMainNav"]:hover{
  opacity: 100%;
}

```
