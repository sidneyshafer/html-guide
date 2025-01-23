# HTML Sandbox for Beginners

>HTML code snippets for learning the basics of HTML.

## Table of Contents
* [Basic HTML Layout](#basic-html-layout)
* [Live Server Extension](#live-server-extension)
* [Meta Tags](#meta-tags)

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
This HTML snippet defines a simple webpage. Below is a brief explanation of the code.

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

[<kbd> <br> Back to Top <br> </kbd>][#table-of-contents]

## Live Server Extension

Live Server Extension for Visual Studio Code by Ritwick Dey - **[GitHub Repository](https://github.com/ritwickdey/vscode-live-server)**

* Launch a development local Server with live reload feature for static & dynamic pages.
* Easier to run, debug, and test HTML webpages.

## Meta Tags
```
<!DOCTYPE html>
<html lang="en">
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
<body>
   
</body>
</html>
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
