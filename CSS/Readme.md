# Introduction to CSS

## Overview

Cascading Style Sheets (CSS) is a style sheet language used to enhance the appearance of HTML elements on a web page. While HTML provides the structural skeleton of a web page, CSS adds visual styling and layout, allowing for a more engaging and user-friendly experience.

## What is CSS?

CSS is not a programming language or a markup language; instead, it is a style sheet language. This means that CSS is designed specifically for styling purposes. It allows developers to selectively style HTML elements, making it a crucial tool in web design and development.

## Key Features of CSS

- **Separation of Content and Presentation**: CSS enables developers to separate the content (HTML) from the presentation (CSS), making it easier to manage and maintain web pages.
- **Styling Options**: CSS provides a wide range of styling options, including colors, fonts, spacing, layout, and responsive design.
- **Selectors and Properties**: CSS uses selectors to target specific HTML elements and apply styles through properties and values.

## Benefits of Using CSS

- **Improved Performance**: By separating styles from content, CSS can reduce page load times and improve performance.
- **Consistency**: CSS allows for consistent styling across multiple web pages, ensuring a uniform look and feel.
- **Flexibility**: CSS can easily be modified and updated without affecting the underlying HTML structure.

# Styling HTML Elements with CSS

## Overview

To style a specific HTML element using CSS, we need three key components:

1. **Selector**: Indicates which HTML element we wish to style (e.g., a paragraph, a heading).
2. **Property**: Specifies which property of the HTML element we want to modify (e.g., color).
3. **Property Value**: Assigns a value to the specified property (e.g., if we want the color to be red, then "red" is our property value).

## Methods of Applying CSS

### 1. Inline Style

Inline styles are used to apply style to a single element within the HTML document. This method is generally the least efficient for styling HTML elements and can be difficult to maintain. Making styling changes may require multiple edits within a single web page, which can be inconvenient.

**Example**:

`<p style="color: red;">This is a red paragraph.</p>`

### 2. Internal Style

Internal styles are used when we want to apply a specific style to a single HTML page. The effect of this style is limited to that particular page. However, using internal style sheets comes with disadvantages; when creating a website with multiple pages, separate internal style sheets must be defined for each page, making it challenging to manage and maintain.

**Example**:
`<head><style> p { color: blue; } </style> </head>`

### 3. External Style

An external style sheet contains CSS in a separate file with a `.css` extension. We create the external style sheet and link it to the HTML document. This approach allows us to target multiple HTML elements using their IDs and classes, enabling a more organized and efficient styling method. A single CSS file can be linked to multiple web pages.

**Example**:

<link rel="stylesheet" type="text/css" href="styles.css">

## Precedence of Styles

When all three styling methods are present in a single HTML document, the following precedence will be observed:

- **Inline Style** > **Internal Style** > **External Style**

This means that if there are conflicting styles, the inline styles will take precedence over internal and external styles.

# CSS Box Model

## Overview

Whenever a browser loads a web page, it considers all HTML elements as rectangular boxes according to the standard CSS box model. The CSS box model indicates the size, position, and other properties such as colors, backgrounds, borders, and more for these boxes.

When a document is rendered in a web browser, each element is represented as a container that consists of the following properties:

## Components of the CSS Box Model

### 1. Content Area

The content area is the innermost section that contains the actual content, such as text or images. It is bound by the content edge, and its dimensions are determined by the width and height of the content box.

### 2. Padding Area

The padding area is a transparent space around the content area that helps clearly demarcate the content boundaries. This area can be visualized as the space around the content area within the border box. Its dimensions are defined by the width and height of the padding box.

### 3. Border Area

The border area is a visible border that encircles the padding and content area. You can define various properties such as color and thickness for the border. Additionally, the border can be made invisible by setting it to hidden.

### 4. Margin Area

The margin area is the space between the border and the outer edge of the box. It is used to create gaps between elements, giving them a more isolated and elegant appearance. The margin area is particularly useful for separating an element from its neighbors.

# Introduction to CSS Positioning

## Overview

CSS positioning allows you to place HTML elements with respect to the document. This feature enables you to take elements out of the normal document layout flow and make them behave differently. In a normal layout flow, HTML elements are stacked one over the other in a specific style. By using CSS positioning, you can define how and where you want to place those elements.

## Positioning Methods

There are five methods to position HTML elements using CSS position properties:

1. **Fixed**
2. **Static**
3. **Relative**
4. **Absolute**
5. **Sticky**

### 1. Static

If you do not use any positioning method, CSS will apply the static method to the element by default. The element will be positioned according to the normal flow of the page. By default, static positioning is applied to every element, meaning it is placed in its normal position within the document layout flow.

### 2. Relative

As the name suggests, when you apply this method, the element is positioned relative to its normal position. If you set an element's position to relative without adding any additional positioning attributes (top, bottom, right, left), there will be no visible change. However, when you add an additional position (e.g., `left: 20px`), the element will move 20 pixels to the right from its normal position. The movement of this element does not affect other elements in the layout.

### 3. Absolute

Using the absolute positioning method, you can place an element with respect to its parent. Positioning occurs relative to the first relatively (or absolutely) positioned parent element. If there is no positioned parent element, the element will be positioned relative to the HTML document (the page itself). An absolutely positioned element no longer exists in the normal document layout flow; instead, it sits on its own layer, which is separate from other layers. This is useful for creating isolated user interface (UI) features, such as pop-up information boxes, that do not interfere with the layout of other elements on the page.

### 4. Fixed

Fixed positioning allows you to fix the position of an element at a specific spot on the HTML page, regardless of scrolling. This method is beneficial when you want to ensure that users do not miss certain content as they navigate the page. For example, fixed positioning can be used for advertisements that remain visible during scrolling or for continuously displaying a company logo.

### 5. Sticky

Sticky positioning is a combination of relative and fixed positions. An element with a sticky position behaves like a relative element until the scroll reaches a specified point, after which it behaves like a fixed element. This can be useful for creating scroll effects in navigation bars or for fixing advertisements on the website after scrolling.

## Fixed vs. Absolute Positioning

You might wonder about the difference between fixed and absolute positioning. The major distinction is that fixed positioning fixes the element relative to the viewport (the device viewing the web page), while absolute positioning modifies the element's position with respect to the nearest parent that has a relative or absolute position. If no such parent exists, the element positions itself relative to the `<html>` element.

# Features Introduced in CSS3

## Overview

CSS3 is the latest version of cascading style sheets, aimed at extending the functionalities of earlier CSS versions. It introduces a variety of exciting features such as rounded corners, shadows, gradients, animations, and more.

## Key Features

### 1. Display

The display property determines how an element is displayed on the web page. Using this property, you can change an inline element to a block-level element and vice versa. There are additional uses for the display property as well. To understand it better, visit the following link: [MDN - display property](https://developer.mozilla.org/en-US/docs/Web/CSS/display).

### 2. Rounded Corners

CSS3 allows you to add rounded corners to your element boxes without requiring additional markup or images.

### 3. Box Shadows

You can create a 3D effect in your HTML elements using the CSS `box-shadow` property, which enhances the visual depth of your designs.

### 4. CSS Colors

With CSS3, you can set colors by encoding RGB (red, green, blue) values using the `rgb()` function. This allows for precise color representation in your designs.

### 5. Text Shadows

You can also apply shadow effects to text to create a 3D appearance by specifying the x, y, and z translations.

### 6. Multiple Background Images

CSS3 enables you to add multiple background images to a single element without the need to create additional elements for each background image. This feature simplifies design and layout processes.

## Conclusion

CSS3 has introduced many other features as well. To learn more about these features, visit the following link: [MDN - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS).

# Introduction to Media Queries

## Overview

What if we want our website to look different on smaller resolution devices compared to larger resolution devices? While it may seem that device-specific code is necessary for this, CSS offers a better solution. It allows us to render web pages with different properties based on device resolution.

## What Are Media Queries?

Media queries are a powerful feature in CSS that enables us to modify our web pages or websites based on the type of device displaying them. They allow us to adjust styles according to specific parameters such as resolution, viewport width, and more.

## How to Use Media Queries

We use the `@media` rule to apply distinct styles to various media types or devices. This functionality allows us to create customized web pages tailored for different types of devices, including tablets, desktops, phones, and screens of varying sizes.

By employing media queries, we can ensure that our web content is responsive and visually appealing across a wide range of devices.
