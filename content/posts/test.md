+++
title = "Markdown Syntax Guide"
date = "2024-11-07"
authors = ["Boxuan Hu"]
+++

This article offers a sample of basic Markdown syntax that can be used in Hugo, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.

<!--more-->

## Headings

You should using `## H2` as your section title, since the file title is `# H1`.

```markdown
### H3
#### H4
##### H5
###### H6
```

## Blockquotes

The blockquote element represents content that is quoted from another source.

### Blockquote without attribution

> Welcome to TechFounders
>
> **Note** that you can use *Markdown syntax* within a blockquote.

### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.</p>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

Hugo supports supports Table, but it's different to original markdown.

   Name | Age
--------|------
  Bob   | 27
  Alice | 23

```markdown
   Name | Age
--------|------
  Bob   | 27
  Alice | 23
```

### Inline Markdown within tables

 Inline     | Markdown  | In                | Table
---------- | --------- | ----------------- | ----------
*italics*  | **bold**  | ~~strikethrough~~ | `code`

```markdown
 Inline     | Markdown  | In                | Table
---------- | --------- | ----------------- | ----------
*italics*  | **bold**  | ~~strikethrough~~ | `code`
```

## Code Blocks

### Code block with backticks and showing highlighted lines

```html {linenos=table, hl_lines=[1,"4-5",8], linenostart=199}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

### Code block indented with four spaces

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

### Code block with Hugo's internal highlight shortcode

{{< highlight html >}}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## List Types

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

* List item
* Another item
* And another item

### Nested list

* Item

1. First Sub-item

2. Second Sub-item

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.
