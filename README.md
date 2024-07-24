# Project 0

Integrating exercise of the concepts seen about HTML5 and CSS3.

## Part 1

### Delivery date (Part 1)

March 21/23, depending on which group you are in.

### Instruction

1. Divide into groups of 2 students.
2. Each group will have to layout a news article (as if it were the page of an online newspaper), creating its content (title, paragraph, images, etc.) based on 3 *random* words that will be assigned to them. .
3. Research [MDN](https://developer.mozilla.org/en-US/) about tags you don't know about.
4. The document **must** include the tags listed in the [structure](#site-structure) below.
5. It is recommended to get inspiration and get ideas from news sites and real articles, for example [this](https://www.lanacion.com.ar/buenos-aires/los-portenos-eligieron-luccianos-como-mejor-heladeria-nid2229133/).
6. To perform this exercise, you will have to [fork](https://help.github.com/en/articles/fork-a-repo) this repository and in *your new copy*, add an `index.html file ` containing the solution.

### Site structure

```
header
    p [1]
    nav
        ul [2]
main               
    article
        section
            h1 [3]
        figure
                img [4]
                figcaption
        section
            p [5]
    aside
        img [6]

footer
    p [7]
    a [8]
    a [9]
```

[1]: Title of the diary.
[2]: List of topics/sections. Here we mark in bold (and in another color) the corresponding one, that is, the current one where we are now.
[3]: Title of the news.
[4]: Image related to the news. It must have the `src` and `alt` attributes!
[5]: Text with the content of the news. It must have links (absolute or relative) somewhere in the text to read more about a topic.
[6]: Advertising/spam image, preferably related to the content of the news.
[7]: Copyright Text.
[8]: Absolute link to some external site.
[9]: Link that takes us to the header of the journal (use `id=header` to identify it).

---

## Part 2

### Delivery date (Part 2)

March 28/30, depending on which group you are in.

### Instruction

For this 2nd part, we are going to start applying styles to our site and make some modifications to our document. At the end a reference image is included to better visualize the modifications.

#### Important

- This 2nd part **DOES NOT** include modifications to the CSS corresponding to the *layout* of the content (the block elements will continue to remain one below the other), that will be left for the 3rd. part of the project.
- The project must be solved with the same group with which you did the 1st part of it.
- Use **Git and GitHub** to collaborate and work together.
- Both team members must present **the same project**, not 2 individual versions.
- **Reuse of styles in CSS** will be evaluated. Also, preferably class selectors are used over any other.

#### CSS Styles

1. *Flatten* list of topics/sections, that is, make the list look horizontal, with the items next to each other.
2. Remove the bullets/vignettes from the list of topics/sections.
3. Define a base size for the font of our document at `18px`.
4. Define a relative size for the `h1` that is 2.25 times larger than the base size.
5. Define a relative size for the `h2` that is 1.75 times larger than the base size.
6. Define a relative size for the `h3` that is 1.4 times larger than the base size.
7. Define the color `#fafafa` as the background color of our site.
8. Define the color `#24292e` as the color for the text of our site (`h1`, `h2`, `h3` and `p`).

#### HTML changes

The structure of our site is going to be slightly modified and look like this
```
header
    p
    nav
        ul
main               
    article
        section
            h1
        figure
            img
            figcaption
        section
            p [10]
            p
            p
            figure
                img
                figcaption
            p [16]
    section [11]
            h2
        article
            h3
            figure
                img
                figcaption
        article
            h3
            figure
                img
                figcaption
    aside
        h3 [12]
        img

hr [15]
footer
    a [13]
    a [14]
    p
```

1. Add a new section [11] that contains the following: 2 `articles`, corresponding to 2 recommended news items (not necessarily related to the one we are reading), with their corresponding titles (`h3`) and descriptive images.
2. Add an `h3` to the `aside` that contains the advertising, with the text `ADVERTISING` [12].
3. The news must contain **at least 3 paragraphs** [10].
4. Add a `p` with a lower margin of `30px` before the first paragraph of the news, in color `#808080` and size `0.75` (relative to the base size), containing the text `<DATE> - <TIME>`, example `March 23, 2019 - 12:36`.
5. Add a 2nd image (with its corresponding caption) related to the news.
6. Add a `p`[16] at the end of the news text, with an upper margin of `25px`, containing the text "By:" followed by absolute links to the GitHub profiles of the project authors ( By: [repo-user-1](#) - [repo-user-2](#)).
7. Add an `hr` [15] before the `footer`, with a top margin of `45px` and the following styles: `border: 0.5px solid #808080;`, width of 80% and opacity `0.3`.
8. Modify the `footer` so that it is similar to the reference image (see below): a `p` with the text Source code: [repo-1](#) | [repo-2](#), which links to the repositories of the site of each author of the project, the Return to the beginning link below (see next item) and the copyright text centered, between both links.
9. The remaining link of the `footer` [14] must continue to be a link with the text "Back to top", which takes us to the `header` of the site.

#### Reference image

![](https://i.imgur.com/f5OIzcq.jpg)

---

## Part 3

### Delivery date (Part 3)

April 11/13, depending on which group you are in.

#### CSS Styles

1. Define some font other than the default for the `p`. This font must be [safe web](http://web.mit.edu/jmorzins/www/fonts.html) to ensure compatibility regardless of the user's operating system.
2. Choose a font from [Google Fonts](http://fonts.google.com) for the `h1` and use it with the `font-weight` corresponding to `bold`.
3. Choose another font from [Google Fonts](http://fonts.google.com) for the `h2` and `h3`. Use it with the `font-weight` corresponding to `bold` (`h1`, `h2/h3` and `p` must have different fonts).
4. Transform the `h3` so that they are always seen in uppercase.
5. Add the corresponding styles to all the images on the site so that they are *responsive*. **Hint:** It is enough to modify their width and height.
6. Modify the style of the links (anchors) on our page, so that they do not have underlining and their color is `#0074c4`.
7. Modify the style of the links (anchors) on our page, so that they have the color `##0098ff` and underlined when you *hover* over them.
8. Float the recommended advertising and news sections to the right so they look like the reference image.
9. Leave a margin of `24px` between the advertising and recommended news sections and the `article` corresponding to the news.
