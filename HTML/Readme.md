# HTML Elements

We can broadly divide HTML elements into the following two categories:

## Block-Level Elements

A block-level element always starts on a new line and stretches to the left and right to the maximum extent possible. Below are some examples of block-level elements:

- `<aside>`
- `<div>`
- `<form>`
- `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`
- `<header>`
- `<li>`
- `<ol>`
- `<p>`
- `<section>`
- `<ul>`

## Inline Elements

An inline element does not start on a new line and only takes up the necessary width. Examples of inline elements include:

- `<a>`
- `<br>`
- `<button>`
- `<img>`
- `<input>`
- `<script>`
- `<select>`
- `<span>`
- `<textarea>`

### Which HTML Elements Take Up Only the Necessary Width?

The answer is **inline elements**. They do not force a new line and take up only as much width as needed by their content.

## Anatomy of Tags

Not all HTML elements necessarily follow the pattern of opening tag + content + closing tag. Some are **self-closing tags**, meaning there is no need for a closing tag.

For example:

- `<br/>`

## HTML Document Structure

HTML consists of various tags that are responsible for a website’s structure. These are the fundamental building blocks of a website. Individual HTML elements are not very useful on their own but work together to structure content.

### Key HTML Tags

- **Document type (`<!DOCTYPE>`)**: This is an instruction that signals the browser about the markup language in which the current page is written.
- **HTML tag (`<html>`)**: The root of the HTML document; it is the container of all other HTML elements.
- **Head tag (`<head>`)**: Contains metadata (data about data) for the HTML document. It includes tags that help the browser understand the document. Metadata in the head section includes:

  - Keywords or a page description for search results.
  - Character set declarations, and more.
  - Note: Content inside the `<head>` tag does not appear on the web page but is used by browsers and search engines.

- **Title tag (`<title>`)**: Defines the title of the document, which shows up in the browser tab when the website is opened.

- **Meta tag (`<meta>`)**: Describes the content characteristics of the web page to the browser. Meta tags are part of the code and do not appear on the actual web page.
