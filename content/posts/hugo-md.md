+++
title = "Markdown on Hugo"
date = "2024-11-07"
authors = ["Boxuan Hu"]
+++

This article provides an example of basic Markdown syntax as used in Hugo, which differs slightly from standard Markdown. 

All content on our blog is rendered from these Markdown files.

<!--more-->

## Headings

You should using `## H2` as your section title, since the file title is `# H1`.

```markdown
### H3
#### H4
##### H5
```

## Blockquotes

The blockquote element represents content that is quoted from another source.


### Blockquote without attribution

You can still use __Markdown syntax__ within a blockquote.

> Welcome to TechFounders
>
> __Note__ that you can use _Markdown syntax_ within a blockquote.


### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.</p>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.


## Tables

Hugo supports supports Table, but the syntax is totally different to original markdown.

   Name | Age
--------|------
  Bob   | 27
  Alice | 23


```markdown
<!-- code in Hugo Markdown-->
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
<!-- code in Hugo Markdown-->
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

You can learn the detailed render syntax [here](https://github.com/TechFounders-Berkeley/TechBlog/tree/main/content/posts)

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

You can learn the detailed render syntax [here](https://github.com/TechFounders-Berkeley/TechBlog/tree/main/content/posts)

## List Types

### Ordered List

1. First item
2. Second item
3. Third item

```markdown
<!-- code in Hugo Markdown-->
1. First item
2. Second item
3. Third item
```

### Unordered List

- List item
- Another item
- And another item

```markdown
<!-- code in Hugo Markdown-->
- List item
- Another item
- And another item
```

### Nested list

- Item

1. First Sub-item

2. Second Sub-item

```markdown
<!-- code in Hugo Markdown-->
- Item

1. First Sub-item

2. Second Sub-item
```

You can learn the detailed render syntax [here](https://github.com/TechFounders-Berkeley/TechBlog/tree/main/content/posts)


## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

