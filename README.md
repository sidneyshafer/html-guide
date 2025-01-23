# HTML Sandbox for Beginners

>HTML code snippets for learning the basics of HTML.

## Table of Contents
* [Basic HTML Layout](#basic-html-layout)
* [Live Server Extension](#live-server-extension)
* [Meta Tags](#meta-tags)
* [Typography - Headings and Paragraphs](#typography---headings-and-paragraphs)
* [Links and Images](#links-and-images)
* [Lists and Tables](#lists-and-tables)

## Basic HTML Layout

```
<!DOCTYPE html>
<html>
   <head>
      <title>My Website</title>
   </head>
   <body>
      <!-- This is a comment -->
      <h1>My Website</h1>
      <p>This is my very first website</p>
   </body>
</html>
```

This HTML snippet defines a simple webpage.

## Code Breakdown

### `<!DOCTYPE html>`
* Declares the document type and version of HTML being used. In this case, it specifies that the document uses HTML5
* Ensures the webpage is rendered correctly by the browser.

### `<html lang="en"></html>`
* The root element containing all other HTML elements.
* HTML elements are nested between opening `<html>` and closing `</html>` tags.
* `</html>` marks the end of an HTML document.
* `lang="en"` specifies the language of the document as English (en). This helps search engines and accessibility tools (like screen readers) understand the primary language of the content.
* Defines the start and end of the HTML document.

### `<head>`
* Contains metadata about the webpage, such as the title, character encoding, styles, and scripts.
* Not visible to users but is critical for search engines and browser functionality.

### `<title>`
* Specifies the title of the webpage.
* This title appears in the browser's tab and is used by search engines to display the page title in search results.
* In this case, `"My Website"` is the title of the webpage.

### `<body>`
* Contains all the content that will be displayed on the webpage.
* Anything inside the `<body>` tag is visible to the user when the webpage is loaded in a browser.

### `<!-- This is a comment -->`
* Commenting in HTML - anything between `<!--` and `-->` is ignored by the browser.
* Useful for adding notes or explanations in the code without affecting the webpage's output.

### `<h1>`
* This tag defines the most important heading on a webpage.
* In this case, `"My Website"` is displayed as the main heading.

### `<p>`
* This tag defines a paragraph of text to be displayed.
* In this example, the text `"This is my very first website"` is displayed as a paragraph.

>See full source code for this section - [01-basic-layout.html](https://github.com/sidneyshafer/html-sandbox/blob/master/01-basic-layout.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Live Server Extension

Live Server Extension for Visual Studio Code by Ritwick Dey - **[GitHub Repository](https://github.com/ritwickdey/vscode-live-server)**

* Launch a development local Server with live reload feature for static & dynamic pages.
* Easier to run, debug, and test HTML webpages.

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Meta Tags
```
<head>
   <meta charset="UTF-8">
   <!-- Important for Responsive Design (different screen sizes)-->
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <!-- meta tags that have to do with search engines -->
   <meta name="description" content="This is my website description">
   <meta name="keywords" content="web development, web design, html, css">
   <!-- Do not index page -->
   <meta name="robots" content="NOINDEX, NOFOLLOW">
   <title>Meta Tags</title>
</head>
```

This HTML snippet demonstrates the use of the `<meta>` tag within the `<head>` section of a webpage. Each `<meta>` tag provides metadata—information about the webpage—that isn't displayed on the webpage itself but is used by browsers, search engines, and other tools.

## Code Breakdown

### `<meta charset="UTF-8">`
* Defines the character encoding for the document as UTF-8.
* Ensures characters from most languages and special symbols are displayed correctly.

### `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
* Improves responsive design by controlling the viewport's width and scaling.
    * `width=device-width`: Sets the width of the viewport to match the device's screen width.
    * `initial-scale=1.0`: Ensures that the page's initial zoom level is set to 1 (no zooming).
* This meta tag is crucial for ensuring that webpages display correctly on mobile and tablet devices.

### `<meta name="description" content="This is my website description">`
* Provides a short description of the webpage's content.
* Used by search engines to generate the snippet shown in search results.
* Helps improve SEO (Search Engine Optimization).

### `<meta name="keywords" content="web development, web design, html, css">`
* List relevant keywords for a webpage.
* Historically used by search engines for indexing - modern search engines no longer prioritize or rely on the keywords meta tag.

### `<meta name="robots" content="NOINDEX, NOFOLLOW">`
* Tells search engines how to handle the page.
    * `NOINDEX`: Prevents the page from being indexed by search engines (it won't appear in search results).
    * `NOFOLLOW`: Instructs search engines not to follow links on this page. 
    * Useful for pages under development or private pages that shouldn't appear in search results.

>See full source code for this section - [03-meta-tags.html](https://github.com/sidneyshafer/html-sandbox/blob/master/03-meta-tags.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Typography - Headings and Paragraphs
```
<!-- Headings -->
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>

<!-- Paragraph -->
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Officia fugiat non temporibus vitae. <strong>Doloribus tempora minus ipsa </strong>eius saepe porro illo, eligendi repudiandae voluptas amet fugiat totam earum quasi, corrupti provident <em>vero dolor </em>sed ipsam voluptatum vel at quibusdam. Adipisci cum consequatur maxime dignissimos assumenda fugiat dolore nam aliquam delectus labore iure laboriosam ullam eos nemo omnis dolores, eaque tenetur vel in <del> hic non!</del> Magnam harum sunt exercitationem doloribus? Illo, minus non.
    <!-- line Break -->
    <br>
    <br>
    Dolor dignissimos cumque laboriosam, temporibus neque assumenda provident culpa dicta atque! Vel, illo? 
    <!-- Horizontal Rule -->
    <hr>
    Harum odit dolorum architecto unde fugit earum impedit. Ad assumenda nihil ex nulla? Assumenda?</p>
```

This snippet of HTML code demonstrates the use of typography-related tags to structure and format textual content of a webpage.

### `<h1> to <h6>` - Headings
Tags: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`
* Define headings of different levels/importance, with `<h1>` being the most important and `<h6>` the least.
* HTML headings provide structure to the content and aid accessibility.
* Search engines prioritize headings to understand the content's hierarchy.
    * `<h1>Heading 1</h1>`: Largest and most prominent.
    * `<h6>Heading 6</h6>`: Smallest and least prominent.

### `<strong>` - Bold
* Inline text formatting applied to parts of a text within a paragraph.
* Indicates strongly emphasized text.
* Typically displayed in bold for emphasis.

### `<em>` - Italics
* Inline text formatting applied to parts of a text within a paragraph.
* Indicates emphasized text that is typically displayed in italic.

### `<del>` - Strikethrough
* Indicates deleted or removed text.
* Displays text with a line through it.

### `<br>` - Line Break
* Creates a single line break in text without starting a new paragraph.
* Used here to add space within the paragraph.

### `<hr>` - Horizontal Rule
* Inserts a thematic break or divider.
* Often used to visually separate sections or ideas.

>See full source code for this section - [04-typography.html](https://github.com/sidneyshafer/html-sandbox/blob/master/04-typography.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Links and Images
```
<!-- External Link -->
<p>
    <a href="http://google.com">Click For Google</a>
</p>
<p>
    <a href="http://google.com" target="_blank">Click For Google</a>
</p>

<!-- Internal Links -->
<p>
    <a href="/04_typography.html">Typography</a>
</p>

<!-- Local Image -->
<img src="/img/sample.jpg" alt="My Image" width="200">

<!-- Remote Images -->
<img src="https://source.unsplash.com/200x200/?building,city" alt="My Image 2">
```

This HTML snippet demonstrates the use of links and images within a webpage.

### `<a>` - Hyperlinks
* The `<a>` tag defines hyperlinks that allow users to navigate to other web pages or resources.

**External Link**
* Example: `<a href="http://google.com">Click For Google</a>`
* Links to an external website.
* Clicking this link takes the user to "http://google.com".

**Internal Link**
* Example: `<a href="/04_typography.html">Typography</a>`
* Links to another page within the same website.

**Attributes**
* `href`: Specifies the URL of the link destination. For internal links, this is usually a relative path to the internal webpage.
* `target="_blank"`: Opens the link in a new tab or window. Useful for external resources that users might want to keep open while continuing on the current page.

### `<img>`
* The `<img>` tag embeds images into a webpage. It is a self-closing tag and requires specific attributes.

**Local Image**
* Example: `<img src="/img/sample.jpg" alt="My Image" width="200">`
* Displays an image stored locally on the server.

**Remote Image**
* Example: `<img src="https://source.unsplash.com/200x200/?building,city" alt="My Image 2">`
* Displays an image loaded from a remote URL.

**Attributes**
* `src`: Specifies the file path to the image.
* `alt`: Provides alternative text for the image, used by screen readers and shown if the image fails to load.
* `width`: Specify image width.
* `height`: Specify image height.

>See full source code for this section - [05-links-and-images.html](https://github.com/sidneyshafer/html-sandbox/blob/master/05-links-and-images.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Lists and Tables

### `<ul>` - Unordered Lists
```
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
    <li>Item 4</li>
</ul>
```
* Defines a list of items without any specific order.
* `<ul>`: Starts the unordered list.
* `<li></li>`: Defines a list item.
* `</ul>`: Ends the unordered list.

### `<ol>` - Ordered Lists
```
<ol type="A">
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
    <li>Item 4</li>
</ol>
```
* Defines a list of items in a specific order.
* `<ol>`: Starts the ordered list.
* `<li></li>`: Defines a list item.
* `</ol>`: Ends the ordered list.
* **Attributes:**
    * `type`: Specifies the style of numbering (e.g., `A` for uppercase letters, `1` for numbers, `i` for Roman numerals).

### Nested List
```
<ul>
    <li>Item 1</li>
    <li>Item 2
        <ul>
        <li>Nested Item 1</li>
        <li>Nested Item 2</li>
        </ul>
    </li>
    <li>Item 3</li>
    <li>Item 4</li>
</ul>
```
* Creates a hierarchy of items within a list.

### Tables
```
<table style="width: 600px;">
    <thead>
        <tr>
        <th>First Name</th>
        <th>Last Name</th>
        <th>Email</th>
        </tr>
    </thead>
    <tbody>
        <tr>
        <td>John</td>
        <td>Doe</td>
        <td>jdoe@gmail.com</td>
        </tr>
        <tr>
        <td>Kate</td>
        <td>Smith</td>
        <td>kate@gmail.com</td>
        </tr>
        <tr>
        <td>Jeff</td>
        <td>Wilson</td>
        <td>jeff@gmail.com</td>
        </tr>
    </tbody>
</table>
```
* Tables are used to organize data into rows and columns for better readability and structure.
* `<table></table>`: Contains all elements for defining a table structure. In this case, includes a style attribute to set the width.
* `<thead></thead>`: Groups the header content. Contains `<tr>` for rows and `<th>` for column headers.
* `<tbody></tbody>`: Groups the main content of the table. Contains rows (`<tr>`), with data cells defined by `<td>`.
* `<tr></tr>`: Defines table rows.
* `<th></th>`: Defines header cells.
* `<td></td>`: Defines data cells.

>See full source code for this section - [06-lists-and-tables.html](https://github.com/sidneyshafer/html-sandbox/blob/master/06-lists-and-tables.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>
