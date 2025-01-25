# HTML Sandbox

>Code snippets for learning the basics of HTML.

## Table of Contents
* [Basic HTML Layout](#basic-html-layout)
* [Live Server Extension](#live-server-extension)
* [Meta Tags](#meta-tags)
* [Typography - Headings and Paragraphs](#typography---headings-and-paragraphs)
* [Links and Images](#links-and-images)
* [Lists and Tables](#lists-and-tables)
* [Forms and Inputs](#forms-and-inputs)
* [Inline vs Block Elements](#inline-vs-block-elements)
* [IDs and Classes](#ids-and-classes)
* [HTML Entities](#html-entities)
* [HTML5 Semantic Tags](#html5-semantic-tags)

## Basic HTML Layout

```html
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

>See full source code for this section [01-basic-layout.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/01-basic-layout.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Live Server Extension

Live Server Extension for Visual Studio Code by Ritwick Dey - **[GitHub Repository](https://github.com/ritwickdey/vscode-live-server)**

* Launch a development local Server with live reload feature for static & dynamic pages.
* Easier to run, debug, and test HTML webpages.

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Meta Tags
```html
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

>See full source code for this section [03-meta-tags.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/03-meta-tags.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Typography - Headings and Paragraphs
```html
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

>See full source code for this section [04-typography.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/04-typography.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Links and Images
```html
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

>See full source code for this section [05-links-and-images.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/05-links-and-images.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Lists and Tables

### `<ul>` - Unordered Lists
```html
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
```html
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
```html
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

>See full source code for this section [06-lists-and-tables.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/06-lists-and-tables.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Forms and Inputs

### `<form>`
* Defines the form element for collecting user input.
* `action`: Specifies the URL where form data will be submitted for processing.

### Form Buttons
**Submit Button**
```
<input type="submit" value="Submit">
```
* Submits the form data to the specified action URL.

**Reset Button**
```
<button type="reset">Reset</button>
```
* Resets all form fields to their default values.

## Form Fields and Inputs
**Text Input**
```
<input type="text" id="name" name="name">
```
* Collects single-line text input.
* `type="text"`: Specifies the input as plain text.
* `id and name`: Used to identify the field and associate it with the `<label>`.

**Number Input**
```
<input type="number" name="age" id="age" min="0" max="100">
```
* Collects a numerical value
* `min` and `max`: Restrict the range of acceptable values.

**Email Input**
```
<input type="email" name="email" id="email" placeholder="Enter an email">
```
* Collects a valid email address.
* `type="email"`: Ensures the input is a properly formatted email.
* `placeholder`: Displays placeholder text in the input field.

**Date Input**
```
<input type="date" name="birthdate" id="birthdate">
```
* Collects a date value.
* In this case, allows users to enter their birthdate using a date picker.

**Radio Buttons**
```html
<div>
    <label for="membership">Membership</label><br>
    <input type="radio" name="membership" value="simple" id="membership"> Simple
    <input type="radio" name="membership" value="standard" id="membership" checked> Standard
    <input type="radio" name="membership" value="super" id="membership"> Super
</div>
```
* Allows selection of a single option from a group.
* `type="radio"`: Defines a radio button.
* `name`: Groups radio buttons (only one radio button can be selected per group).
* `checked`: Pre-selects a default option.

**Checkboxes**
```html
<div>
    <label for="membership">Hobbies</label><br>
    <input type="checkbox" name="hobbies" value="bike" id="hobbies"> Bike
    <input type="checkbox" name="hobbies" value="drawing" id="hobbies" checked> Drawing
    <input type="checkbox" name="hobbies" value="cooking" id="hobbies"> Cooking
</div>
```
* Allows multiple selections from a list of options.
* `type="checkbox"`: Defines a checkbox input.
* `checked`: Pre-selects the option.

**Textarea**
```html
<textarea name="message" id="message" cols="50" rows="10"></textarea>
```
* Collects multi-line text input.
* `cols`: Specifies the width of the text area.
* `rows`: Specifies the height of the text area.

**Select Dropdown**
```html
<select name="gender" id="gender">
    <option value="male">Male</option>
    <option value="female" selected>Female</option>
    <option value="other">Other</option>
</select>
```
* Provides a dropdown menu for selecting a single option.
* `<option>`: Defines individual options.
* `selected`: Pre-selects the default option.

**Datalist**
```html
<input list="states" name="state" id="state">
<datalist id="states">
    <option value="Alaska"></option>
    <option value="Alabama"></option>
</datalist>
```
* Provides autocomplete suggestions for input.
* `list`: Associates the `<input>` with the `<datalist>` by `id`.
* `<option>`: Defines items for the input.

>See full source code for this section [07-forms-input.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/07-forms-input.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## Inline vs Block Elements

**Block-Level Elements**
* Block-level elements occupy the full width of their parent container and start on a new line. They create a new line in the document flow.
* Examples include: `<p>`, `<ul>`, `<li>`.
* Allow child elements (both block and inline elements) inside.
* Block elements define the structure of the document, creating vertical layouts.

**Inline Elements**
* Inline elements only take up as much width as necessary and do not start on a new line.
* Examples include: `<a>`, `<strong>`, `<em>`.
* Remains "inline" within the text or other content.
* Cannot contain block-level elements but can contain other inline elements.
* Inline elements enhance or modify content within block elements without disrupting the flow.

**Comparison Table**
| Feature | Block Elements | Inline Elements |
| --------| -------------- | --------------- |
| Does the element start on a new line? | Yes | No |
| Does the element occupy the full width of containing element? | Yes | No |
| How do nested elements operate? | Can contain block and inline | Can only contain inline |
| Examples | `<p>`, `<ul>`, `<li>` | `<a>`, `<strong>`, `<em>` |

>See full source code for this section [08-block-inline.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/08-block-inline.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## IDs and Classes

**ID**
* A unique identifier for a specific HTML element.
* Only one element should have a given `id` on a page.
* Example: `<div id="main-header">`
* Used for:
    * Targeting specific elements in CSS for unique styling.
    * Selecting elements in JavaScript for manipulation.
    * Creating bookmarks for navigation (e.g., href="#main-header").

**Class**
* A reusable identifier applied to multiple elements for grouping or shared styling.
* Example: `<div class="card">`
* Usage:
    * Can be used on multiple elements.
    * Used to apply the same CSS styling to multiple elements or group them logically.

>See full source code for this section [09-id-class.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/09-id-class.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## HTML Entities

**What are HTML Entities?**
* HTML entities are special codes used to display characters that:
    1. **Have a reserved purpose in HTML** (e.g., `<`, `>`).
    2. **Cannot be typed directly** (e.g., non-breaking spaces, special symbols).
* **Syntax**: Begins with `&`, followed by the entity name (e.g., `&nbsp;`) or numerical code (e.g., `&#160;`), and ends with a semicolon (`;`).

**Entity Breakdown**
| Name | Symbol(s) | Purpose |
| ---- | --------- | ------- |
| Non-Breaking Space | `&nbsp;` | Adds extra spaces between words or elements. |
| Greater Than | `&gt;` and `&#62;` | Displays the `>` (greater-than) symbol. |
| Less Than | `&lt;` and `&#60;` | Displays the `<` (less-than) symbol. |
| Copyright  | `&copy;` | Displays the copyright symbol (`©`). |
| Registered Trademark  | `&reg;` | Displays the registered trademark symbol (`®`). |
| Cent Sign  | `&cent;` | Displays the cent sign (`¢`). |
| Pound Sterling  | `&pound;` | Displays the pound sterling symbol (`£`). |
| Yen/Yuan  | `&yen;` | Displays the yen/yean symbol (`¥`). |
| Euro  | `&euro;` | Displays the euro symbol (`€`). |
| Spade  | `&spades;` | Displays the spade symbol (`♠`). |
| Club  | `&clubs;` | Displays the club symbol (`♣`). |
| Heart  | `&hearts;` | Displays the heart symbol (`♥`). |
| Diamond  | `&diams;` | Displays the diamond symbol (`♦`). |
| <  | `&lt;` | Displays the code entity for `<`. |
| >  | `&gt;` | Displays the code entity for `>`. |

* `<kbd>`: Displays text in a monospace font, indicating a keyboard input.

>See full source code for this section [10-entities.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/10-entities.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>

## HTML5 Semantic Tags

Semantic tags provide meaning to the structure, making it easier for browsers, developers, and assistive technologies (like screen readers) to interpret the content.
* Assistive technologies can better interpret the structure and purpose of the content.
* Search engines can prioritize and understand content structure more effectively.
* Semantic tags make the HTML code easier to read and maintain.
* Aligns with modern web standards, ensuring better browser compatibility.

### `<header>`
```html
<header id="header" class="card">
    <h1>My Website</h1>
    <p>Just Another Website</p>
</header>
```
* Represents the header section of the page or a section. 
* Typically contains introductory content like a logo, site title, or tagline.

### `<main>`
```html
<main id="main">
    ...
</main>
```
* Contains the primary content of the document. 
* It is intended to hold the central information relevant to the page.

### `<section>`
```html
<section id="welcome" class="card">
   <h2>Welcome To Our Website</h2>
   ...
</section>
<section id="blog">
   <p>From Our Blog</p>
   ...
</section>
```
* Represents a standalone section of content, often with its own heading. 
* Useful for grouping related content.

### `<article>`
```html
<article class="article">
   <h3>Article 1</h3>
   ...
</article>
<article class="article">
   <h3>Article 2</h3>
   ...
</article>
```
* Represents a self-contained piece of content that could stand alone (e.g., a blog post, news article).
* Used for individual blog articles, each with a title and content.

### `<aside>`
```html
<aside id="sidebar" class="card">
   <h3>Navigation</h3>
   <nav>
      <ul id="main-nav">
         <li><a href="index.html">Home</a></li>
         <li><a href="about.html">About</a></li>
         <li><a href="contact.html">Contact</a></li>
      </ul>
   </nav>
   ...
</aside>
```
* Represents content related to the main content, such as sidebars, advertisements, or additional navigation links.

### `<nav>`
```html
<nav>
   <ul id="main-nav">
      <li><a href="index.html">Home</a></li>
      <li><a href="about.html">About</a></li>
      <li><a href="contact.html">Contact</a></li>
   </ul>
</nav>
```
* Represents a navigation block containing links to other sections or pages.

### `<footer>`
```html
<footer id="footer">
   <p class="text-center">Copyright &copy; My Website 2020</p>
</footer>
```
* Represents the footer of the page or a section. 
* Typically includes copyright info, legal disclaimers, or contact details.

>See full source code for this section [11-html5-semantic-elements.html](https://github.com/sidneyshafer/html-sandbox/blob/master/src/11-html5-semantic-elements.html)

<kbd> <br> [Back to Top](#table-of-contents) <br> </kbd>
