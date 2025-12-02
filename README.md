# 100 Must-Know HTML & CSS Interview Questions in 2025

<div>
<p align="center">
<a href="https://www.interview247.net/modules/html_css">
<img src="https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/github-blog-img%2Fweb-and-mobile-development-github-img.jpg?alt=media&token=1b5eeecc-c9fb-49f5-9e03-50cf2e309555" alt="web-and-mobile-development" width="100%">
</a>
</p>

#### You can also find all 100 answers here 👉 [Interview247 - HTML & CSS](https://www.interview247.net/modules/html_css)

<br>

## 1. What is HTML and why is it important in web development?

HTML, or HyperText Markup Language, is the standard language for creating the structure and content of web pages. It is fundamentally important because it acts as the skeleton of a website, providing the semantic meaning and foundational layer that browsers render and that other technologies like CSS and JavaScript build upon.

HTML, which stands for **HyperText Markup Language**, is the standard and foundational language for creating the structure and content of web pages and web applications.

The name itself breaks down its function: "HyperText" refers to the links that connect web pages to one another, creating the web, while "Markup Language" means it uses tags to describe or "mark up" different parts of the content, so a browser knows how to display them.

### The Skeleton of the Web

A common and effective analogy is to think of a website as a person. In this analogy:

- **HTML is the skeleton**: It provides the essential structure and holds all the content. Without it, there is nothing.
- **CSS is the skin and clothing**: It provides the styling, presentation, and visual layout, making the structure look good.
- **JavaScript is the muscles and brain**: It adds interactivity, dynamic behavior, and complex functionality.

This hierarchy shows why HTML is so important—it is the absolute foundation upon which everything else is built. CSS and JavaScript need an HTML structure to target and modify.

### Why HTML is Crucial

1.  **Provides Semantic Meaning**: Good HTML uses tags that describe the content's purpose. For example, `<h1>` is a main heading, `<p>` is a paragraph, and `<nav>` is a set of navigation links. This semantic structure is vital for search engine optimization (SEO) and accessibility.
2.  **Ensures Accessibility (A11y)**: Assistive technologies, like screen readers for visually impaired users, rely on the semantic structure of HTML to interpret a page and convey its content accurately.
3.  **Acts as a Universal Standard**: Every web browser, regardless of the device or operating system, understands HTML. This shared standard ensures that web content can be rendered consistently for users everywhere.

### Basic HTML Document Example

Here’s a look at a fundamental HTML structure to illustrate how it works:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Page Title</title>
  </head>
  <body>
    <h1>This is a Main Heading</h1>

    <p>This is a paragraph. It contains the page's text content.</p>

    <a href="https://www.example.com">This is a link</a>
  </body>
</html>
```

In summary, HTML is not just a part of web development; it's the starting point and the core framework. A strong command of HTML is essential for building websites that are not only functional but also accessible, maintainable, and well-ranked by search engines.

<br>

## 2. What is the role of the &lt;!DOCTYPE&gt; declaration?

The &lt;!DOCTYPE&gt; declaration is an instruction that must be the first line in an HTML document. Its primary role is to inform the browser which version of HTML the page is written in. This is crucial because it ensures the browser renders the page in "standards mode," leading to consistent and predictable behavior, rather than falling back to "quirks mode," which can cause layout inconsistencies.

The `<!DOCTYPE>` declaration, short for "document type declaration," is a crucial instruction for the web browser. It is not an HTML tag, but rather a preamble that must be the very first thing in an HTML document, appearing even before the `<html>` tag. Its primary role is to tell the browser's rendering engine which version of HTML (or XML) the document is written in.

### Triggering Browser Rendering Modes

The most significant function of the DOCTYPE is to control the browser's rendering mode. Without a DOCTYPE, or with an incorrect one, browsers enter what is known as **"quirks mode."**

- **Quirks Mode:** This is a backward-compatibility mode that mimics the rendering behavior of older browsers like Internet Explorer 5. It can cause CSS to be applied inconsistently and lead to unpredictable layouts. It exists to prevent old websites from breaking in modern browsers.
- **Standards Mode:** When a valid DOCTYPE is present, the browser renders the page according to the W3C and WHATWG web standards. This ensures more predictable, consistent, and correct behavior across different browsers, which is essential for all modern web development.

#### The Modern HTML5 DOCTYPE

In HTML5, the DOCTYPE declaration was greatly simplified to be easy to remember and use. It is case-insensitive:

```html
<!DOCTYPE html>
```

This simple declaration tells all modern browsers to render the page in standards mode using the current HTML specification.

#### Historical Context: Older DOCTYPEs

To appreciate the simplicity of the HTML5 version, it's helpful to see what came before. Older versions of HTML, like HTML 4.01 or XHTML 1.0, required long and complex DOCTYPEs that referenced a specific Document Type Definition (DTD) file.

```html
<!-- HTML 4.01 Strict DTD -->
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">

<!-- XHTML 1.0 Transitional DTD -->
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```

### Summary

In short, you should always start every HTML document with `<!DOCTYPE html>`. It is a mandatory first line that guarantees your page is rendered in standards mode, providing a stable and predictable foundation for your HTML and CSS.

<br>

## 3. Difference between HTML tag and HTML element?

An HTML tag is the syntax used to create an element, consisting of a keyword in angle brackets like &lt;p&gt; and &lt;/p&gt;. An HTML element is the complete structure created by the tags, including the start tag, the content, and the end tag. Essentially, tags are the markers, and the element is the final object they create.

The fundamental difference is that an **HTML tag** is the syntax used to mark the beginning and end of an element, while an **HTML element** is the complete component created by the tags, including its content. In simple terms, tags are the instructions, and the element is the resulting object in the Document Object Model (DOM).

### HTML Tag

A tag is a special keyword enclosed in angle brackets, like `<p>`. Most tags come in pairs:

- A **start tag** (or opening tag), like `<h1>`, marks the beginning of an element.
- An **end tag** (or closing tag), like `</h1>`, marks its end. The end tag is identical to the start tag but with a forward slash before the tag name.

Some tags, known as _empty_ or _void_ tags, do not have an end tag because they don't contain any content, such as `<br>` or `<img>`.

### HTML Element

An HTML element consists of the start tag, the content, and the end tag. It represents a complete structural unit of an HTML document.

#### Example of an Element

```html
<p>This is the content of the paragraph element.</p>
```

In this example, `<p>` is the start tag, `</p>` is the end tag, and the text in between is the content. The entire line forms a single paragraph element.

### Key Differences at a Glance

| Aspect         | HTML Tag                                                      | HTML Element                                                        |
| :------------- | :------------------------------------------------------------ | :------------------------------------------------------------------ |
| **Definition** | The syntax marker used to define an element.                  | The complete structural component, including tags and content.      |
| **Syntax**     | Enclosed in angle brackets, e.g., `<div>` and `</div>`.       | Consists of a start tag, content, and an end tag.                   |
| **Purpose**    | To instruct the browser on how to format and display content. | To create the structure and objects of the webpage (the DOM nodes). |

### Nested Elements

Elements can also be nested inside other elements, which is how the hierarchical structure of an HTML document is built.

```html
<div>
  <h1>This is a heading</h1>
  <p>This is a paragraph inside the div.</p>
</div>
```

Here, the `<div>` element contains an `<h1>` element and a `<p>` element. The tags define where each element begins and ends, but the elements themselves are the actual structural blocks.

<br>

## 4. Difference between block, inline, and inline-block elements?

Block elements start on a new line and take up the full available width, respecting all sizing and spacing properties. Inline elements flow within the text, take up only the necessary width, and ignore vertical margins, width, and height. Inline-block is a hybrid, flowing like an inline element but allowing control over its dimensions and spacing like a block element.

Certainly. The difference between `block`, `inline`, and `inline-block` is fundamental to understanding page layout in CSS. It all comes down to how an element behaves in terms of page flow, sizing, and spacing.

### Block-level Elements

Block-level elements are the foundational building blocks of a layout. By default, they begin on a new line and take up the full width available to them, stretching to fill their parent container. They create a "block" structure in the document.

- **Page Flow:** Always starts on a new line.
- **Sizing:** Respects `width` and `height` properties. If no width is set, it defaults to 100% of its container.
- **Spacing:** Respects `margin` and `padding` on all four sides (top, right, bottom, and left).

###### Common Examples:

- `<div>`
- `<p>`
- `<h1>` - `<h6>`
- `<form>`
- `<ul>`, `<ol>`, `<li>`

### Inline Elements

Inline elements are the opposite. They do not start on a new line and only occupy as much width as their content requires. They are designed to flow "in line" with text and other inline elements.

- **Page Flow:** Does not start on a new line; it sits alongside other inline elements and text.
- **Sizing:** The `width` and `height` properties have no effect. The element's size is determined by its content.
- **Spacing:** Respects horizontal `margin` and `padding` (left and right), but vertical (top and bottom) margins and padding are ignored and will not affect the layout of surrounding elements.

###### Common Examples:

- `<span>`
- `<a>`
- `<img>`
- `<strong>`
- `<em>`

### Inline-Block Elements

This is a hybrid of the other two. An element with `display: inline-block` gives you the best of both worlds: it flows horizontally like an inline element but allows you to control its dimensions and spacing like a block element.

- **Page Flow:** Does not start on a new line, allowing other elements to sit next to it.
- **Sizing:** Respects `width` and `height` properties.
- **Spacing:** Respects `margin` and `padding` on all four sides.

This is particularly useful for creating navigation bars or grids of items where you want elements to sit side-by-side while also controlling their size and spacing precisely.

### Comparison Summary

| Property                            | Block          | Inline           | Inline-Block     |
| :---------------------------------- | :------------- | :--------------- | :--------------- |
| Starts on a new line?               | Yes            | No               | No               |
| Respects width & height?            | Yes            | No               | Yes              |
| Respects vertical margin & padding? | Yes            | No               | Yes              |
| Default Width                       | 100% of parent | Width of content | Width of content |

### Code Example

```css
/* A block element will take up its own line. */
.box-1 {
  display: block;
  width: 200px;
  height: 100px;
  margin: 10px;
  background-color: lightblue;
}

/* An inline element flows with text and ignores width/height. */
.link-1 {
  display: inline;
  margin: 20px; /* Vertical margin will be ignored */
  background-color: lightyellow;
}

/* An inline-block element sits inline but respects dimensions. */
.button-1 {
  display: inline-block;
  width: 150px;
  height: 50px;
  margin: 10px;
  background-color: lightgreen;
}
```

<br>

## 5. What is the difference between &lt;head&gt; and &lt;body&gt; in HTML?

The &lt;head&gt; element contains metadata about the HTML document, such as the title and links to stylesheets; this content is not displayed on the page. The &lt;body&gt; element contains all the visible content that the user interacts with, like text, images, and links.

In an HTML document, the **&lt;head&gt;** and **&lt;body&gt;** elements serve two distinct and fundamental purposes. The &lt;head&gt; section is for metadata and setup information that the browser uses, while the &lt;body&gt; section holds the actual content that is rendered for the user to see and interact with.

### The &lt;head&gt; Element: The Brains

The &lt;head&gt; element is a container for metadata (data about the document) and is placed between the &lt;html&gt; tag and the &lt;body&gt; tag. Nothing inside the &lt;head&gt; is rendered in the main browser window, but it provides crucial instructions to the browser.

##### Common elements found in the &lt;head&gt; include:

- **&lt;title&gt;:** Sets the title of the page, which appears in the browser tab and in search-engine results.
- **&lt;meta&gt;:** Provides information like character encoding (e.g., UTF-8), viewport settings for responsive design, and keywords or descriptions for SEO.
- **&lt;link&gt;:** Used to link to external resources, most commonly CSS stylesheets to style the page.
- **&lt;script&gt;:** Embeds or references executable client-side scripts, usually JavaScript. While scripts can be placed in the body, it's common to load them in the head.

### The &lt;body&gt; Element: The Face

The &lt;body&gt; element defines the document's main content. Everything inside this tag—such as text, headings, images, links, tables, and paragraphs—is the content that gets displayed to the user in the browser window.

### Key Differences at a Glance

| Aspect              | &lt;head&gt;                                         | &lt;body&gt;                                     |
| :------------------ | :--------------------------------------------------- | :----------------------------------------------- |
| **Purpose**         | Contains metadata and resource links                 | Contains the visible page content                |
| **Visibility**      | Not displayed on the page (except for the title)     | All content is rendered in the browser window    |
| **Typical Content** | `<meta>`, `<title>`, `<link>`, `<style>`, `<script>` | `<h1>`, `<p>`, `<img>`, `<div>`, `<a>`           |
| **Uniqueness**      | There must be only one &lt;head&gt; per document     | There must be only one &lt;body&gt; per document |

### Structural Example

Here is a basic HTML document structure showing how they work together:

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Metadata goes here -->
    <meta charset="utf-8" />
    <title>Page Title (Shows in Tab)</title>
    <link rel="stylesheet" href="styles.css" />
  </head>

  <body>
    <!-- Visible content goes here -->
    <h1>This is a Visible Heading</h1>
    <p>This is a paragraph that users can read.</p>
  </body>
</html>
```

<br>

## 6. How do &lt;head&gt; and &lt;body&gt; work together in an HTML document?

The `&lt;head&gt;` element contains metadata for the browser, such as the page title, character set, and links to external resources like CSS files. The `&lt;body&gt;` element contains the actual content that is rendered and displayed to the user. In essence, the `&lt;head&gt;` sets up the context and necessary resources, while the `&lt;body&gt;` holds the visible structure and content that uses them.

The **&lt;head&gt;** and **&lt;body&gt;** tags are the two direct children of the &lt;html&gt; element, and they serve distinct but complementary roles. They work together by separating the document's metadata and setup instructions from its actual visible content.

#### The &lt;head&gt; Element: The Document's Metadata

The &lt;head&gt; section contains information _about_ the webpage rather than the content of the page itself. This metadata is processed by browsers and search engines but is not displayed to the user (with the exception of the &lt;title&gt; tag). Think of it as the backstage area, preparing everything for the main show.

- **&lt;title&gt;:** Sets the text for the browser tab, bookmarks, and search engine results.
- **&lt;meta&gt;:** Provides crucial information like character encoding (e.g., `UTF-8`), viewport settings for responsive design, and descriptions for SEO.
- **&lt;link&gt;:** Used to connect to external resources, most importantly CSS stylesheets which define the visual presentation of the page.
- **&lt;script&gt; and &lt;style&gt;:** Used to include JavaScript and internal CSS, respectively, which add behavior and styling to the content.

#### The &lt;body&gt; Element: The Document's Content

The &lt;body&gt; section contains all the content that is actually visible to the user in the browser window. This is the main stage where the text, images, videos, links, and other elements that form the webpage are placed.

#### How They Cooperate

The &lt;head&gt; sets the stage for what the &lt;body&gt; presents. The browser parses the &lt;head&gt; first to understand the page's title, apply styling rules from linked CSS files, and load necessary scripts. Then, it renders the content within the &lt;body&gt;, applying the rules and resources it gathered from the &lt;head&gt;.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Webpage</title>
    <!-- The link below tells the browser how to style the body's content -->
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Welcome!</h1>
    <p>This content is styled by the rules found in styles.css.</p>
  </body>
</html>
```

#### Comparison Table

| Aspect         | &lt;head&gt;                                     | &lt;body&gt;                        |
| :------------- | :----------------------------------------------- | :---------------------------------- |
| **Purpose**    | Metadata and resource linking                    | Visible page content                |
| **Visibility** | Not displayed on the page (except &lt;title&gt;) | Rendered in the main browser window |
| **Analogy**    | The page's "brain"                               | The page's "body" or "face"         |

<br>

## 7. What is the role of the &lt;title&gt; tag?

The &lt;title&gt; tag defines the document's title that is displayed in the browser tab, in bookmarks, and on search engine results pages. It is a required element within the &lt;head&gt; section and is critical for both user experience and SEO, as it provides a clear and concise description of the page's content.

The `&lt;title&gt;` tag is a required HTML element that defines the title of the document. Its content is not displayed on the page itself but is used in several key places to identify the document, making it crucial for user experience, SEO, and accessibility.

#### Where the Title Appears

- **Browser Tab/Window:** It's the text shown on the browser tab, helping users identify the page when multiple tabs are open.
- **Search Engine Results Pages (SERPs):** Search engines like Google use the title's content as the main clickable headline for a search result.
- **Browser Bookmarks/Favorites:** When a user bookmarks a page, the title is used as the default name.

#### Correct Usage

The `&lt;title&gt;` tag must be placed within the `&lt;head&gt;` section of an HTML document, and only one title element is allowed per document.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Document Title Goes Here</title>
  </head>
  <body>
    <h1>Page Content</h1>
  </body>
</html>
```

#### Why the &lt;title&gt; Tag is Important

1.  **Search Engine Optimization (SEO):** It is a critical on-page SEO factor. A well-written title with relevant keywords helps search engines understand the page's content and significantly impacts search rankings.
2.  **User Experience (UX):** A clear title helps users with navigation and orientation. It provides immediate context, allowing them to easily find the correct browser tab or bookmark.
3.  **Accessibility:** Screen readers announce the page title when a user lands on a page. This is often the first piece of information an accessibility user receives, so it's vital for providing context.

<br>

## 8. What is the purpose of the &lt;meta&gt; tag?

The &lt;meta&gt; tag provides metadata about the HTML document that isn't displayed on the page itself. Its primary purposes are to define the character set, set the viewport for responsive design, and provide descriptive information for search engines and social media platforms.

The `&lt;meta&gt;` tag is a fundamental HTML element used within the `&lt;head&gt;` section to provide metadata about the HTML document. This metadata is not displayed on the page itself but is machine-parsable, providing information for browsers, search engines, and other web services.

### Core Purpose and Attributes

The primary role of `&lt;meta&gt;` is to define properties of the document like its character set, page description, keywords, author, and viewport settings. This is primarily handled through these key attributes:

- **`charset`**: Specifies the character encoding for the document. This is a critical declaration for ensuring text displays correctly.
- **`name`**: Used for document-level metadata, paired with the `content` attribute. Common names include `description`, `keywords`, `author`, and `viewport`.
- **`content`**: Provides the value for the metadata specified by the `name` or `http-equiv` attribute.
- **`http-equiv`**: Used to simulate an HTTP response header, which can control browser actions like page refresh or content type.

#### Key Use Cases with Examples

Here are some of the most common and important applications of the `&lt;meta&gt;` tag.

##### 1. Character Set Declaration

This is arguably the most crucial meta tag. It ensures the browser correctly interprets the characters on the page, preventing issues with special characters or different languages.

```html
<!-- Sets the character encoding to UTF-8 -->
<meta charset="UTF-8" />
```

##### 2. Viewport for Responsive Design

This tag is essential for modern, responsive web design. It controls the page's dimensions and scaling on different devices, especially mobile phones.

```html
<!-- Ensures the page width matches the device width and sets the initial zoom level -->
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

##### 3. Search Engine Optimization (SEO)

Search engines use meta tags to understand and rank a page's content. The `description` is particularly important as it's often used as the preview snippet in search results.

```html
<!-- A brief description of the page's content for search engine results -->
<meta
  name="description"
  content="This page provides a comprehensive guide to HTML meta tags."
/>
<!-- Keywords are less impactful for major search engines today but can still be included -->
<meta name="keywords" content="HTML, Meta Tags, SEO, Web Development" />
```

##### 4. Social Media Sharing (Open Graph & Twitter Cards)

Specialized meta tags, like those for the Open Graph protocol, control how your content appears when shared on social media platforms like Facebook, LinkedIn, or Twitter. They allow you to specify the title, description, and preview image.

```html
<!-- Open Graph (Facebook, etc.) -->
<meta property="og:title" content="The Ultimate Guide to Meta Tags" />
<meta
  property="og:description"
  content="Learn everything you need to know about using meta tags for SEO and social sharing."
/>
<meta property="og:image" content="https://example.com/images/meta-guide.jpg" />
<meta property="og:url" content="https://example.com/meta-guide" />

<!-- Twitter Cards -->
<meta name="twitter:card" content="summary_large_image" />
```

In summary, the `&lt;meta&gt;` tag is a versatile and powerful tool that provides essential information to configure the document, improve its SEO, and control its presentation across different platforms and devices.

<br>

## 9. What is the difference between absolute and relative URLs?

An absolute URL is a full web address, including the protocol (https://) and domain name, making it globally unique and independent of the current location. A relative URL is a partial address that points to a resource in relation to the current page, which makes it shorter and more portable for internal linking within the same website.

The core difference lies in how they define the path to a resource. An **absolute URL** is a complete address, including the protocol and domain, which points to the same location regardless of context. A **relative URL** is a partial address that points to a resource in relation to the current document's location.

#### Absolute URLs

An absolute URL contains all the information needed to locate a resource. It starts with the protocol (like `https://`), followed by the domain name, and then the full path to the resource. It is unambiguous and will always point to the same file, no matter where the link is located.

##### Example:

```html
<a href="https://www.example.com/products/item1.html">View Product</a>
```

##### When to Use Absolute URLs:

- When linking to an external website or a resource on a different domain.
- When defining the canonical URL or the `<base>` href for a page.
- In content that might be syndicated or viewed outside of your website, like in an RSS feed or an email.

#### Relative URLs

A relative URL provides a partial path to a resource from the current page's directory. Because it doesn't specify the protocol or domain, the browser assumes the resource is on the same server. This makes the website much more portable—if you change your domain name, you don't have to update any internal links.

##### Examples:

If our current page is `/about/team.html`:

- To link to a file in the _same directory_ (e.g., `/about/contact.html`):
  ```html
  <a href="contact.html">Contact Us</a>
  ```
- To link to a file in a _subdirectory_ (e.g., `/about/history/2020.html`):
  ```html
  <a href="history/2020.html">Our History</a>
  ```
- To link to a file in a _parent directory_ (e.g., `/index.html`):
  ```html
  <a href="../index.html">Back to Home</a>
  ```

#### Key Differences Summarized

| Aspect          | Absolute URL                            | Relative URL                                    |
| :-------------- | :-------------------------------------- | :---------------------------------------------- |
| **Structure**   | Full address (protocol + domain + path) | Partial address (path relative to current file) |
| **Use Case**    | Linking to external sites               | Linking to internal pages and assets            |
| **Portability** | Site will break if domain changes       | Links remain intact if domain changes           |

In practice, the standard is to use **relative URLs for all internal links** to ensure the site is easy to maintain and deploy, and use **absolute URLs only when linking to external resources**.

<br>

## 10. How do you create a hyperlink in HTML?

To create a hyperlink in HTML, you use the anchor `&lt;a&gt;` tag. The most important attribute is `href`, which specifies the destination URL. The text or content placed between the opening `&lt;a&gt;` and closing `&lt;/a&gt;` tags becomes the clickable link for the user.

In HTML, a hyperlink is created using the anchor tag, which is represented by `<a>`. This is one of the most fundamental tags in HTML, as it's what makes the web a "web" of interconnected documents.

### Core Syntax

The basic structure of a hyperlink involves the opening `<a>` tag, a crucial attribute called `href`, the visible link text, and the closing `</a>` tag.

```html
<a href="https://www.example.com">Visit Example.com</a>
```

- `<a>`: The anchor tag itself.
- `href`: The "hypertext reference" attribute, which specifies the destination URL or path.
- `Visit Example.com`: The content inside the tag, which becomes the clickable part of the link.
- `</a>`: The closing tag.

### Types of URLs in the `href` Attribute

The `href` attribute can point to different kinds of resources:

1.  **Absolute URLs:** A full web address to a different website.
    `<a href="https://www.google.com">Go to Google</a>`
2.  **Relative URLs:** A path to a file within the same website. This is useful for internal navigation.
    `<a href="/about.html">About Us</a>`
3.  **Fragment Identifiers (Anchor Links):** A link to a specific section on the same page, which requires the target section to have an `id` attribute.
    `<a href="#section-two">Jump to Section Two</a>`
4.  **Other Protocols:** You can also link to other resources, like triggering an email client.
    `<a href="mailto:contact@example.com">Email Us</a>`

### Other Important Attributes

Besides `href`, several other attributes are important for usability, accessibility, and security.

| Attribute | Description                                                                                                                                                                                                            |
| :-------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `target`  | Specifies where to open the linked document. The most common value is `_blank`, which opens the link in a new tab or window. The default is `_self`.                                                                   |
| `title`   | Provides extra information about the link, which typically appears as a tooltip when the user hovers over it. This can be helpful for accessibility.                                                                   |
| `rel`     | Defines the relationship between the current page and the linked document. When using `target="_blank"`, it is critical for security to add `rel="noopener noreferrer"` to prevent potential security vulnerabilities. |

#### Complete Example

Here is an example combining these attributes for a secure, user-friendly external link:

```html
<a
  href="https://developer.mozilla.org/"
  target="_blank"
  rel="noopener noreferrer"
  title="Visit the Mozilla Developer Network"
>
  MDN Web Docs
</a>
```

<br>

## 11. How do you include an image in HTML and what is alt used for?

You include an image using the &lt;img&gt; tag with the 'src' attribute to define the image path. The 'alt' attribute is essential for accessibility, providing a text alternative for screen readers. It also displays if the image fails to load and helps search engines understand the image content.

To include an image in an HTML document, you use the `<img>` tag, which is a self-closing or void element. This tag requires at least two attributes to function correctly: `src` to specify the image source path and `alt` to provide alternative text.

### Key Attributes

- **`src` (Source):** This attribute is mandatory and specifies the URL or path to the image file you want to display. The path can be relative to the HTML file or an absolute URL pointing to an image on another server.
- **`alt` (Alternative Text):** This attribute provides descriptive text that serves several critical purposes. It is considered essential for accessibility and modern web standards.

#### The Purpose of the 'alt' Attribute

The `alt` attribute is crucial for three main reasons:

1.  **Accessibility:** Screen readers read the alt text aloud to visually impaired users, allowing them to understand the content and context of the image. Without it, these users would have no way of knowing what the image conveys.
2.  **Usability:** If an image fails to load due to a broken link, slow connection, or user settings, the browser will display the alt text in its place. This ensures the user still gets the information the image was meant to provide.
3.  **SEO (Search Engine Optimization):** Search engine crawlers cannot "see" images, so they rely on alt text to understand the image's content. Well-written alt text can help your page rank better in image search results.

#### Code Example

```html
<!-- This image has descriptive alt text -->
<img
  src="images/golden-retriever-puppy.jpg"
  alt="A golden retriever puppy playing in a grassy field."
/>

<!-- For a purely decorative image, the alt attribute is left empty -->
<img src="images/decorative-border.png" alt="" />
```

In summary, while the `src` attribute tells the browser _what_ image to load, the `alt` attribute describes _what_ the image is about, ensuring the content is accessible and robust for all users and search engines.

<br>

## 12. Difference between &lt;div&gt; and &lt;span&gt;?

The primary difference is their display model: a `&lt;div&gt;` is a block-level element used for grouping larger sections of content and creating layouts, as it starts on a new line. In contrast, a `&lt;span&gt;` is an inline element used to style or target a small, specific piece of content within a line, without disrupting the document's flow.

The fundamental difference between a **&lt;div&gt;** and a **&lt;span&gt;** is that they are different types of elements by default. A &lt;div&gt; is a _block-level_ element used to group larger sections of content for layout purposes, while a &lt;span&gt; is an _inline_ element used to wrap smaller, specific pieces of content, like text or icons, for styling or targeting.

### The &lt;div&gt; Element: The Block Container

A &lt;div&gt; (or "division") element is a generic block-level container. This means:

- It will always start on a new line in the document.
- It will take up the full width of its parent container by default.
- It's primarily used to group other elements together to create structural sections of a webpage, such as headers, content areas, or footers, which can then be styled with CSS.

#### Example:

```html
<!-- Each div creates a separate block -->
<div style="border: 1px solid blue;">
  <h4>This is a section.</h4>
  <p>It contains a heading and a paragraph, grouped together.</p>
</div>
<div style="border: 1px solid green;">
  <p>This is another, completely separate section.</p>
</div>
```

### The &lt;span&gt; Element: The Inline Container

A &lt;span&gt; is a generic inline container. This means:

- It does not start on a new line.
- It only takes up as much width as its content requires.
- It’s used to apply styles or scripts to a small, specific part of content without disrupting the overall layout of the text or elements around it.

#### Example:

```html
<p>
  Most of this sentence is standard text, but this
  <span style="color: red; font-weight: bold;">one part</span>
  has been styled differently without breaking the line.
</p>
```

### Comparison Table

| Feature           | &lt;div&gt;                                                   | &lt;span&gt;                                                          |
| :---------------- | :------------------------------------------------------------ | :-------------------------------------------------------------------- |
| **Display Type**  | block-level                                                   | inline                                                                |
| **Visual Effect** | Creates a "break" before and after the element.               | Flows "in line" with the rest of the content.                         |
| **Common Use**    | Page layout, content sections, containers for other elements. | Styling text, adding icons, targeting a small piece of content.       |
| **Content**       | Can contain both block-level and inline elements.             | Best used for phrasing content (text, images, other inline elements). |

In essence, you should choose a **&lt;div&gt;** when you need to create a structural division or section on the page, and a **&lt;span&gt;** when you simply need to hook into a piece of content within a line to style it.

<br>

## 13. What are semantic HTML elements? Give examples.

Semantic HTML elements are tags that clearly describe their meaning and purpose to both the browser and the developer, such as &lt;header&gt;, &lt;nav&gt;, and &lt;article&gt;. They improve accessibility, SEO, and code readability by providing a structural context for the content, unlike non-semantic elements like &lt;div&gt; or &lt;span&gt; which are for styling and grouping only.

Semantic HTML elements are tags that clearly describe their meaning and purpose to both the browser and the developer. Unlike non-semantic elements like `<div>` or `<span>` which are purely for styling and grouping, semantic tags provide a structural context for the content within them. Using them makes the web more accessible, improves SEO, and makes the codebase more readable.

### Key Benefits of Using Semantic HTML

- **Accessibility:** Assistive technologies, like screen readers, use semantic elements to understand the page structure and help users navigate. For example, a screen reader can announce a `<nav>` element as a navigation block, allowing a user to easily find or skip it.
- **SEO:** Search engines can better parse the content and understand its hierarchy and importance, which can lead to better search rankings. A search engine gives more weight to content inside an `<article>` or an `<h1>` than a generic `<div>`.
- **Maintainability:** Semantic code is largely self-documenting and easier for developers to read and understand. It's much clearer to see a layout made of `<header>`, `<main>`, and `<footer>` than a series of nested divs with IDs.

### Common Semantic vs. Non-Semantic Elements

Historically, developers relied heavily on generic `<div>` tags with IDs or classes to structure pages. HTML5 introduced a rich set of semantic elements to provide a better, more meaningful structure out-of-the-box.

| Semantic Element | Purpose                                                             | Common Non-Semantic Alternative |
| :--------------- | :------------------------------------------------------------------ | :------------------------------ |
| `<header>`       | Introductory content, navigation, or branding.                      | `<div id="header">`             |
| `<nav>`          | A set of major navigation links.                                    | `<div id="nav">`                |
| `<main>`         | The main, unique content of the page.                               | `<div id="main-content">`       |
| `<article>`      | Self-contained, distributable content (e.g., a blog post).          | `<div class="article">`         |
| `<section>`      | A thematic grouping of content.                                     | `<div class="section">`         |
| `<aside>`        | Content tangentially related to the main content (e.g., a sidebar). | `<div id="sidebar">`            |
| `<footer>`       | Footer content for a document or section (e.g., author, copyright). | `<div id="footer">`             |

#### Example: Page Structure Comparison

Here is a comparison of a webpage layout using the old, non-semantic approach versus the modern, semantic approach.

##### Non-Semantic Layout (The "div-itis" approach)

```html
<div id="header">
  <h1>My Website</h1>
</div>
<div id="nav">
  <ul>
    ...
  </ul>
</div>
<div id="main">
  <div class="article">
    <h2>Article Title</h2>
    <p>Article content...</p>
  </div>
</div>
<div id="footer">
  <p>&copy; 2024 My Website</p>
</div>
```

##### Semantic Layout (The Modern Way)

```html
<header>
  <h1>My Website</h1>
</header>
<nav>
  <ul>
    ...
  </ul>
</nav>
<main>
  <article>
    <h2>Article Title</h2>
    <p>Article content...</p>
  </article>
</main>
<footer>
  <p>&copy; 2024 My Website</p>
</footer>
```

In summary, using semantic HTML is a modern best practice that creates more meaningful, accessible, and maintainable web pages. It's about choosing the right element for the right job, which provides clear benefits to users, search engines, and developers alike.

<br>

## 14. What are self-closing tags in HTML?

Self-closing tags, also known as void elements, are HTML tags that don't need a separate closing tag because they cannot contain any content. Their behavior is defined entirely through their attributes. Common examples include the `&lt;img&gt;` tag for images, `&lt;br&gt;` for line breaks, and `&lt;input&gt;` for form fields.

In HTML, self-closing tags, more formally known as **void elements** or **empty elements**, are elements that do not have a separate closing tag. They are written this way because they are designed to be standalone and cannot contain any content or other elements within them.

### Syntax

In HTML5, the syntax is simply the tag name inside angle brackets. While in older XHTML, it was mandatory to include a trailing slash before the closing bracket (e.g., `<br />`), this is now optional in HTML5. However, many developers still include it for readability or XML compatibility.

```html
<!-- Standard HTML5 syntax -->
<br />
<img src="path/to/image.jpg" alt="An example image" />

<!-- XHTML-style syntax (also valid in HTML5) -->
<br />
<hr />
```

### Common Examples of Self-Closing Tags

Here are some of the most frequently used void elements:

- **&lt;br&gt;**: Creates a line break within text.
- **&lt;hr&gt;**: Represents a thematic break between paragraph-level elements, often rendered as a horizontal rule.
- **&lt;img&gt;**: Embeds an image. Its behavior is defined by attributes like `src` and `alt`.
- **&lt;input&gt;**: Creates an interactive control for a web form to accept data from the user.
- **&lt;link&gt;**: Specifies a relationship between the current document and an external resource, most commonly a CSS stylesheet.
- **&lt;meta&gt;**: Provides machine-readable metadata about the document, such as character set or viewport settings.

### Comparison: Self-Closing vs. Regular Tags

| Aspect      | Self-Closing (Void) Tag                          | Regular Tag                                           |
| :---------- | :----------------------------------------------- | :---------------------------------------------------- |
| Example     | `<img>`, `<br>`                                  | `<p>`, `<div>`                                        |
| Content     | Cannot contain any content or child elements.    | Designed to contain text, other elements, or both.    |
| Closing Tag | Does not have a closing tag (e.g., no `</img>`). | Must have a corresponding closing tag (e.g., `</p>`). |

Understanding this distinction is crucial for writing valid and well-structured HTML. Using a self-closing tag correctly ensures the document is parsed as expected by the browser without any unintended layout issues.

<br>

## 15. Difference between &lt;section&gt;, &lt;article&gt;, and &lt;aside&gt;?

The key difference is semantic. A `&lt;section&gt;` groups related content, an `&lt;article&gt;` is for self-contained, distributable content like a blog post, and an `&lt;aside&gt;` is for tangentially related content like a sidebar. Their correct use is vital for accessibility and creating a logical document outline.

The **&lt;section&gt;**, **&lt;article&gt;**, and **&lt;aside&gt;** elements are all HTML5 semantic tags used to structure a document, but they serve different purposes based on the content's meaning and relationship to the page.

### The &lt;section&gt; Element

A **&lt;section&gt;** is a thematic grouping of content. It's used to group related content together when there isn't a more specific semantic element available. A general rule is that a section should always have a heading (h1-h6) as a child element, which identifies the purpose of that section.

```html
<!-- A section for contact information -->
<section>
  <h2>Contact Us</h2>
  <p>You can reach us by phone or email.</p>
  <!-- More contact details here -->
</section>
```

### The &lt;article&gt; Element

An **&lt;article&gt;** represents a complete, self-contained piece of content that should be independently distributable or reusable. This is the key characteristic; if you could syndicate the content in an RSS feed, it's likely an article.

- **Examples:** A blog post, a news story, a forum post, or a user-submitted comment.

```html
<!-- A single blog post -->
<article>
  <h2>The Future of Web Development</h2>
  <p>Web development continues to evolve at a rapid pace...</p>
  <p>Published on <time datetime="2023-10-27">October 27, 2023</time></p>
</article>
```

### The &lt;aside&gt; Element

An **&lt;aside&gt;** contains content that is only tangentially related to the main content it is placed within. It's often represented as a sidebar, a call-out box, or a pull quote.

- **Examples:** A list of related links, an author's biography in a post, or advertisements.

```html
<article>
  <h2>Understanding CSS Grid</h2>
  <p>CSS Grid is a powerful two-dimensional layout system...</p>
  <aside>
    <h4>Related Reading</h4>
    <ul>
      <li>A Complete Guide to Flexbox</li>
      <li>New Features in CSS</li>
    </ul>
  </aside>
</article>
```

### Key Differences and How to Choose

| Element           | Purpose                                             | Key Question to Ask                                                                |
| :---------------- | :-------------------------------------------------- | :--------------------------------------------------------------------------------- |
| `&lt;section&gt;` | Groups thematically-related content.                | Is this a distinct block of related content that needs a heading?                  |
| `&lt;article&gt;` | Encapsulates self-contained, distributable content. | Could this content stand alone in an RSS feed or be reused elsewhere?              |
| `&lt;aside&gt;`   | Contains tangentially-related side content.         | Is this content complementary but not essential to understanding the main content? |

In summary, the choice depends on semantics. An **&lt;article&gt;** is for standalone content, a **&lt;section&gt;** is for grouping parts of a larger whole, and an **&lt;aside&gt;** is for related but separate side content.

<br>

#### Explore all 100 answers here 👉 [Interview247 - HTML & CSS](https://www.interview247.net/modules/html_css)

<br>

<a href="https://www.interview247.net/modules/html_css">
<img src="https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/github-blog-img%2Fweb-and-mobile-development-github-img.jpg?alt=media&token=1b5eeecc-c9fb-49f5-9e03-50cf2e309555" alt="web-and-mobile-development" width="100%">
</a>
</p>
