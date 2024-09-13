---
title: Components to be used in Posts
date: 2024-09-11 14:39:44
categories:
tags:
author: Eric Prem Raju
avatar: https://hexo.io/logo.svg
thumbnail: https://hexojs.github.io/hexo-theme-landscape/css/images/banner.jpg
---
# Headings

| Syntax | Output |
|---|---|
| `# 'heading-name'` | <h1>Level 1</h1> |
| `## 'heading-name'` | <h2>Level 2</h2> |
| `### 'heading-name'` | <h3>Level 3</h3> |
| `#### 'heading-name'` | <h4>Level 4</h4> |
| `##### 'heading-name'` | <h5>Level 5</h5> |
| `###### 'heading-name'` | <h6>Level 6</h6> |

a. There are no spaces between the `#` in syntax
b. There is space between `#` and `heading-name`.
c. Note that `Level 1` and `Level 2` Heading has underline.
d. Each level will show on the right side contents bar.

# Emphasis

## Bold

| Syntax | Output |
|---|---|
| `**This is bold**` | **This is bold** |
| `__This is bold__` | __This is bold__ |

* Don't do the following. Markdown applications don’t agree on how to handle underscores in the middle of a word

| Syntax | Output |
|---|---|
| `This__is__bold`, instead do this `This**is**bold` | This__is__bold, instead do this This**is**bold |

## Italics

| Syntax | Output |
|---|---|
| `*This is italics*` | *This is italics* |
| `_This is italics_` | _This is italics_ |

* Do not use underscores in the middle of a sentence or word.

## Bold and Italics

| Syntax | Output |
|---|---|
| `***This text is bold and italics***` | ***This text is bold and italics*** |
| `___This text is bold and italics___` | ___This text is bold and italics___ |
| `**_This text is bold and italics_**` | **_This text is bold and italics_** |
| `__*This text is bold and italics*__` | **_This text is bold and italics_** |
| `This text is***bold and italics***` | This text is***bold and italics*** |

## Underline

| Syntax | Output |
|---|---|
| `<u>This text is underlined</u>` | <u>This text is underlined</u> |

## Strikethrough

| Syntax | Output |
|---|---|
| `~~This text is strikethrough~~` | ~~This text is strikethrough~~ |

## Highlight

| Syntax | Output |
|---|---|
| `This text is <mark>highlighted</mark>` | This text is <mark>highlighted</mark> |

## Blockquotes

Syntax
Use `>` before a paragraph for blockquotes
`> This is a blockquote`

Output:
> This is a blockquote

### Blockquotes with Multiple Paragraphs

Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs.

Syntax
`> This is paragraph 1`
`>`
`> This is paragraph 2`

Output:

> This is paragraph 1
>
> This is paragraph 2

### Nested Blockquotes

Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.

Syntax
`> This is paragraph 1`
`>`
`>> This is paragraph 2`
`>`
`> This is paragraph 3`

Output:

> This is paragraph 1
>
>> This is paragraph 2
>
> This is paragraph 3

### Blockquotes with Other Elements

With bold

`> **This is bold in blockquotes**`
> **This is bold in blockquotes**

With underline

`> <u>This is underlined</u>`
> <u>This is underlined</u>

and so on.

## Subscript

| Syntax | Output |
|---|---|
| `H<sub>2</sub>O` | H<sub>2</sub>O |

## Superscript

| Syntax | Output |
|---|---|
| `x<sup>2</sup>` | x<sup>2</sup> |

# Lists

## Ordered Lists

Syntax

> 1. apple
> 2. ball
> 3. cat
> 4. dog

Output:

1. apple
2. ball
3. cat
4. dog

* Note that in the syntax the first letter starts with `1`, rest of the numbering can be anything. Example below:

> 1. apple
> 3. ball
> 5. cat
> 9. dog

1. apple
3. ball
5. cat
9. dog

### Indented List 

- Use `TAB` key on the keyboard twice if you want to keep same numbering.
- Use `Space` key four times or one `TAB` for numbering change

Output with two `TAB`:
1. apple
2. ball
3. cat
        1. bat
        2. rat
3. dog

Output with four `Space` or one `TAB`:
1. apple
2. ball
3. cat
    1. bat
    2. rat
3. dog

## Unordered List

Use `-` at the beginning to denote an unordered list 

Syntax
` - apple`
` - ball`
` - cat`
` - dog`
` - elephant`

Output
- apple
- ball
- cat
- dog
- elephant

### Indented List

Similar to ordered list style

### Starting Unordered List Items With Numbers
If you need to start an unordered list item with a number followed by a period, you can use a backslash `\` to escape the period.

Syntax
` - 10 apple`
` - 20\. ball`
` - cat`
` - dog`
` - elephant`

Output
- 10 apple
- 20\. ball
- cat
- dog
- elephant

# Code Blocks

## Backticks

| Syntax | Output |
|---|---|
| ``Use single backtick to denote `code`.`` | Use single backtick to denote `code`. |

## Code Block

Use a single `TAB` or 4 `Space` for code block

Output

    <HTML>
        <Body>
        Test
        </Body>
    </HTML>

# Links

## Links with title (hidden links)

| Syntax | Output |
|---|---|
| `[This is text](https://kkavion.com)` | [This is text](https://kkavion.com) |

## Links without title

| Syntax | Output |
|---|---|
| `https://kkavion.com` | https://kkavion.com |
| `info@kkavion.com` | info@kkavion.com |

* Links can also be formatted using Emphasis(shown above)

## Images

Use `!` exclamation mark followed by alternative text in square brackets `[]` and then the link to the image file in parenthesis `()`

| Syntax | Output |
|---|---|
| `![KHW Logo](/images/ih-logo.webp)` | ![KHW Logo](/images/ih-logo.webp) |

- Markdown doesn't support image sizing so to resize the image you will have to use HTML tags

| Syntax | Output |
|---|---|
| `<img src="/images/ih-logo.webp" height="" width="150" alt="KHW Logo">` | <img src="/images/ih-logo.webp" height="100" width="150" alt="KHW Logo"> |

# Tables
To add a table, use three or more hyphens (---) to create each column’s header, and use pipes (|) to separate each column.

Syntax

`| Syntax      | Description |`
`|---|---|`
`| Header      | Title       |`
`| Paragraph   | Text        |`

Output

| Syntax      | Description |
|---|---|
| Header      | Title       |
| Paragraph   | Text        |

## Alignment

Use the (:) with (---) to specify alignment in the columns

Syntax

`| Left Align | Center Align | Right Align |`
`|:---|:---:|---:|`
`| Left | Center | Right |`

Output

| Left Align | Center Align | Right Align |
|:---|:---:|---:|
| Left | Center | Right |

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```