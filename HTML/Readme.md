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

## HTML Tags I

- **Body tag (`<body>`)**: Contains the main content of the web page. It is the container for all other elements that describe the structure of the website.
- **Heading tags (`<h1>` to `<h6>`)**: Define the headings of content. These vary in font size, with `<h1>` being the largest and `<h6>` the smallest. The tag is used based on the hierarchy of importance.

- **Paragraph tag (`<p>`)**: Defines a paragraph of text.

- **List tags:**

  - **Unordered list (`<ul>`)**: Displays items in bullet points.
  - **Ordered list (`<ol>`)**: Displays items in a numbered list.
  - **List item (`<li>`)**: Defines individual list items within `<ul>` or `<ol>` tags.

- **Anchor tag (`<a>`)**: Allows you to insert hyperlinks. It has an `href` attribute that specifies the link destination.

- **Break tag (`<br>`)**: Adds a line break within content.

- **Horizontal rule tag (`<hr>`)**: Inserts a horizontal line to divide content visually.

### Comment in HTML

You can add a comment in an HTML document using the following syntax:

`<!-- This is a comment -->`

# HTML Tags II

## Image Tag (`<img>`)

The `<img>` tag is used to insert an image into a web page. It has the following attributes:

- **`src`**: Specifies the path from which the image is to be loaded.
- **`alt`**: Provides alternate text that is displayed if the image fails to load.

### Example:

`<img src="path/to/image.jpg" alt="Description of image">`

## HTML Ids and Classes

### HTML Id

The `id` attribute is used to define an element uniquely. By using `id`, we can target a specific element in a particular HTML document.

### HTML Classes

We can have multiple elements with the same class name. The `class` attribute is used when we want the same operation to be performed over multiple elements in a particular HTML document. HTML classes signify elements over which we can add some functionality or properties. The elements belonging to one class can then exhibit the specified behavior, allowing the same property to be applied to all of them at once.

## HTML Forms

HTML forms are used to collect information from the user that can be sent to the server for further processing.

### Input Tag

The `<input>` tag allows the user to insert data into an editable field. There are multiple types of input tags. Some of them are as follows:

- `<input type="text">`: Shows a single-line text input field.
- `<input type="checkbox">`: Provides a checkbox.
- `<input type="button">`: Displays a clickable button.
- `<input type="radio">`: Defines a radio button.
- `<input type="email">`: Allows users to enter an email address.
- `<input type="number">`: Enables numerical input.
- `<input type="password">`: Hides the input text for secure entry.
- `<input type="file">`: Lets users upload files.
- `<input type="submit">`: Submits the form.
- `<input type="reset">`: Resets the form fields to their default values.
- `<input type="date">`: Provides a date picker.
- `<input type="time">`: Allows users to input a specific time.
- `<input type="color">`: Opens a color picker.

### Label Tag

To avoid confusion for users about what each input field is for, we use the `<label>` tag. The `<label>` tag is used to provide information to the user about what the input field is about. It helps to identify the type of data that needs to be filled in the input field.

### Main Elements of HTML Forms

- **`<input>`**: As the name suggests, this element helps the user to insert data. The type of data is determined by the `type` attribute of the input element. It can be text, button, checkbox, etc.
- **`<label>`**: This is used to give a label to the form elements, aiding the user in identifying the type of data that needs to be filled in the input field.

## HTML Semantic Tags

Semantic tags are those tags that describe the meaning to both developers and browsers. But why do we need HTML semantics in the first place?

HTML semantics helps developers easily identify the type of data that will be populated. It is easier to find portions written with semantic tags compared to scrolling through endless lines of code in long files.

Lastly, when we use semantic tags, it helps various search engines recognize important keywords and can help increase the reach of the web page.

### Common Semantic Tags

- **`<header>`**: The header tag is used to define the header section of the document. It usually contains the introductory part of the website, such as the logo, title of the website, and some navigational links.
- **`<section>`**: The section tag is used to create a section in a document. The most important use of the section tag is to group a generic block of similar content.
- **`<nav>`**: The navbar tag is used to define the section containing the navigation links, which helps the user navigate to different pages or sections of the website.
- **`<footer>`**: The footer tag is used to define the footer section of the website. It may contain pieces of information such as copyright, contact details, and links to privacy policies.

- **`<article>`**: The article tag is used to define an independent piece of content, such as a blog post or news article, that can stand alone and be distributed or reused.

- **`<aside>`**: The aside tag is used for content that is tangentially related to the content around it, often used for sidebars or supplementary information.

- **`<figure>`**: The figure tag is used to encapsulate media content such as images, diagrams, or videos, along with a caption (`<figcaption>`).

- **`<main>`**: The main tag represents the main content of the document, excluding headers, footers, navigation, and sidebars.

- **`<time>`**: The time tag is used to represent a specific period in time, which can be useful for displaying dates and times in a machine-readable format.

Using these semantic tags not only improves the structure of your HTML but also enhances accessibility and search engine optimization (SEO).
