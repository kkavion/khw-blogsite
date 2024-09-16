---
title: Theme Redefine components
date: 2024-09-16 17:20:49
categories:
tags:
author: Eric Prem Raju
avatar: https://hexo.io/logo.svg
thumbnail: https://hexojs.github.io/hexo-theme-landscape/css/images/banner.jpg
---

# Notes

## Large Note Block

Format: (`notel` stands for `note large`, easy to remember, can also be written as `note-large`)

Syntax
```
{% notel default fa-info info %}
text 1
text 2
text 3
{% endnotel %}
```

Output
{% notel default fa-info info %}
text 1
text 2
text 3
{% endnotel %}

| Parameter |	Description	| Optional Values|
|---|---|---|
| Color	| Style or color of the note block | `blue`, `red`, `cyan`, `purple`, `orange`, `yellow`, `green` and other colors |
| Custom Icon | Custom icon, optional | The second part of the icon name from Fontawesome, for example, `fa-image` |

## Small Note Block

Syntax
```
{% note default fa-info info %}
text 1
{% endnote %}
```

Output
{% note default fa-info %}
text 1
{% endnote %}

| Parameter |	Description	| Optional Values|
|---|---|---|
| Style/Color	| Style or color of the note block | `success` `default` `primary` `info` `warning` `danger` `tip` `question` and `blue` `red` `cyan` `purple` `orange` `yellow` `green` and other colors |
| Custom Icon | Custom icon, optional | The second part of the icon name from Fontawesome, for example, `fa-image` |

# Buttons

Syntax

`{% btn [optional size]::[name]::[url]::[optional icon] %}`

Output
{% btn [optional size]::[name]::[url]::[optional icon] %}

<u>Options</u>

`size`:
> center, regular, large, center large, center regular

`icon`:
> Fontawesome icon names, such as fa-solid, fa-house.

# Folding or Accordian

Syntax
```
{% folding [colour]::[title] %}
Content
{% endfolding %}
```

Output
{% folding blue::Title %}
Content
{% endfolding %}

Colour List: `yellow`, `blue`, `green`, `red`, `orange`, `pink`, `cyan`, `white`, `black`, `gray`

# Tabs

Syntax
```
{% tabs First unique name %}
    <!-- tab First Tab-->
        **This is Tab 1.**
    <!-- endtab -->
 
    <!-- tab Second Tab-->
        **This is Tab 2.**
 
        This is Tab 2.
    <!-- endtab -->
 
    <!-- tab Third Tab-->
        **This is Tab 3.**
 
        This is Tab 3.
 
        This is Tab 3.
    <!-- endtab -->
{% endtabs %}
```

Output
{% tabs First unique name %}
<!-- tab First Tab-->
**This is Tab 1.**
<!-- endtab -->
 
<!-- tab Second Tab-->
**This is Tab 2.**
 
This is Tab 2.
<!-- endtab -->
 
<!-- tab Third Tab-->
**This is Tab 3.**
 
This is Tab 3.
 
This is Tab 3.
<!-- endtab -->
{% endtabs %}

# Article attributes

## Sticky Posts on Homepage

Sticky posts show up on the top of the list on homepage and they are permanent on that position

To define sticky, add `sticky` attribute to the post page settings with a value

Syntax
```
---
title: Post Title
date: 
tags: 
categories: 
sticky: 999
---
```

# Author

Adds an author name for the post

Syntax
 `author: Author Name`

# Banner for Post

Adds an banner behind the post title

Syntax
`banner: "image url"`

# Thumbnail for Post

Adds an thumbnail for homepage posts

Syntax
`thumbnail: "image url"`

# Categories

Sets the categories for the posts

Syntax
`categories: Food`

# Avatar

Adds images for the Authors

Syntax
`Avatar: "image url"`

# Excerpt

If you want to customize the article summary on the homepage

Syntax
`excerpt: "Summary"`

If you don't want excerpt on homepage the set `excerpt: false`