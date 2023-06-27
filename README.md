## Arc Browser Boosts ⭐

Snippets to 'boost' websites on [Arc browser](https://arc.net/)

### How to add a boost

1. On Arc browser go to arc://boost/new
2. Select a template (Style, Replace, Inject, or Custom)
3. Enter the URL of the targeted website
4. Copy in the boost

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

Simplifies the TikTok sidebar by removing the 'Following accounts' list

| Template | URL                |
| -------- | ------------------ |
| Style    | https://tiktok.com |

<details>
<summary>View</summary>


</details>

```css
[class*="DivUserContainer"] {
  visibility: hidden;
}
```