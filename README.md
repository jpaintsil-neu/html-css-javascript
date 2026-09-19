# CS 5610 — HTML, CSS, and JavaScript Self-Assessment

A web development self-assessment project created for **CS 5610: Web Development** at Northeastern University.

This project demonstrates foundational HTML and CSS concepts, including semantic page structure, search engine optimization (SEO), HTML layout techniques, the CSS box model, font sizing units, and CSS positioning.

## Live Website

View the deployed project using GitHub Pages:

**https://jpaintsil-neu.github.io/html-css-javascript/**

## Repository

**GitHub Repository:**  
https://github.com/jpaintsil-neu/html-css-javascript

---

## Project Overview

The goal of this project is to demonstrate an understanding of core web-development concepts using HTML and CSS.

The webpage was built as a single-page website containing several demonstrations and explanations of fundamental web-development techniques.

The project covers:

- Semantic HTML page structure
- Navigation using anchor links
- Common HTML elements
- Search Engine Optimization (SEO)
- HTML block and inline elements
- A 3 × 3 layout using only `<div>` and `<span>`
- The CSS box model
- Absolute and relative font-size units
- Inline CSS styling
- CSS positioning
- A fixed footer
- Git and GitHub version control
- GitHub Pages deployment

---

## Technologies Used

The project currently uses:

- **HTML5** — page structure and content
- **CSS3** — presentation, layout, box-model demonstrations, and positioning
- **Git** — local version control
- **GitHub** — remote source-code hosting
- **GitHub Pages** — public website deployment
- **Visual Studio Code** — development environment

The repository also contains a `package.json` file. Node.js is not required to run the current static webpage, but the file may support future JavaScript or Node-based development as the course progresses.

---

## Project Structure

```text
html-css-javascript/
│
├── index.html
├── styles.css
├── package.json
└── README.md
```

### `index.html`

Contains the structure and content of the webpage, including:

- SEO metadata
- Navigation
- Main page heading
- HTML fundamentals
- SEO explanations
- 3 × 3 HTML layout
- Box-model examples
- Font-size demonstrations
- CSS positioning examples
- Footer

### `styles.css`

Contains the external CSS used to demonstrate:

- CSS Grid for the box-model gallery
- Border values
- Margin values
- Padding values
- Relative positioning
- Absolute positioning
- Sticky positioning
- Fixed positioning
- Footer presentation

### `package.json`

Contains basic npm project metadata. It is not required for the current static HTML/CSS implementation but can be used if the repository is expanded with JavaScript or Node.js functionality later.

---

# Assignment Requirements

## 1. HTML Page Structure

The webpage contains a semantic HTML structure with:

- Navigation bar
- Main content area
- One primary `<h1>` heading
- Four primary content sections
- Subheadings
- Footer

Example page hierarchy:

```text
<body>
│
├── <nav>
│
├── <main>
│   │
│   ├── <h1>
│   │
│   ├── HTML Fundamentals
│   ├── Search Engine Optimization
│   ├── CSS Box Model
│   └── CSS Fonts and Positioning
│
└── <footer>
```

The navigation bar uses internal anchor links to move between sections of the webpage.

For example:

```html
<a href="#html-basics">HTML</a>
<a href="#seo">SEO</a>
<a href="#box-model">Box Model</a>
<a href="#css-demo">CSS Demo</a>
```

Each link points to a unique section ID.

---

## 2. Ten Useful HTML Tags

The project identifies and explains ten commonly used HTML elements.

| HTML Tag | Purpose |
|---|---|
| `<div>` | Generic block-level container |
| `<span>` | Generic inline container |
| `<a>` | Creates hyperlinks |
| `<p>` | Creates paragraphs |
| `<img>` | Displays images |
| `<section>` | Defines a section of related content |
| `<nav>` | Identifies navigation content |
| `<header>` | Represents introductory content |
| `<footer>` | Represents footer content |
| `<form>` | Creates a form for collecting user input |

These elements represent some of the most common building blocks used when constructing webpages.

---

## 3. HTML 3 × 3 Layout

The webpage contains a simple Tic-Tac-Toe-style 3 × 3 layout created without:

- HTML tables
- CSS Grid
- CSS Flexbox
- CSS-based layout rules

Instead, the demonstration uses only `<div>` and `<span>` elements.

The `<div>` elements form the rows because they behave as block-level elements.

The `<span>` elements appear within each row because they behave as inline elements.

Conceptually:

```text
<div>
    <span>Cell</span>
    <span>Cell</span>
    <span>Cell</span>
</div>

<div>
    <span>Cell</span>
    <span>Cell</span>
    <span>Cell</span>
</div>

<div>
    <span>Cell</span>
    <span>Cell</span>
    <span>Cell</span>
</div>
```

This exercise demonstrates the behavioral difference between block-level and inline HTML elements.

---

# Search Engine Optimization (SEO)

The project includes a section explaining important HTML elements and metadata related to SEO.

## Page Title

```html
<title>CS 5610 Web Development | John Paintsil</title>
```

The `<title>` element defines the title of the webpage.

It appears in the browser tab and may also be used by search engines when displaying the page in search results.

---

## Character Encoding

```html
<meta charset="UTF-8">
```

The character encoding declaration tells the browser how webpage characters should be interpreted.

UTF-8 supports a large range of letters, symbols, and international characters.

---

## Viewport

```html
<meta
    name="viewport"
    content="width=device-width, initial-scale=1.0"
>
```

The viewport metadata helps webpages display correctly on devices with different screen sizes.

`width=device-width` makes the webpage match the width of the device.

`initial-scale=1.0` establishes the initial browser zoom level.

---

## Meta Description

```html
<meta
    name="description"
    content="CS 5610 self-assessment demonstrating HTML, CSS, SEO, the box model, font units, and CSS positioning."
>
```

The meta description provides a concise summary of the webpage.

Search engines may use this description when presenting the page in search results.

---

## Robots Metadata

```html
<meta name="robots" content="index, follow">
```

The robots metadata provides instructions to search-engine crawlers.

- `index` permits the webpage to be indexed.
- `follow` permits crawlers to follow links found on the page.

---

## Heading Hierarchy

The webpage uses heading elements to organize content logically:

```text
<h1> — Main page heading
<h2> — Major sections
<h3> — Subsections
<h4> — Additional subsection detail
```

A logical heading hierarchy improves page organization for users and provides semantic structure that can also help search engines understand the page.

---

# CSS Box Model

The project demonstrates the four major areas of the CSS box model:

```text
Margin
  Border
    Padding
      Content
```

### Content

The actual text or content contained inside an element.

### Padding

The space between an element's content and its border.

### Border

The visible boundary surrounding the element's padding and content.

### Margin

The space outside the element's border that separates the element from other elements.

---

## Box Model Gallery

The project contains nine example boxes organized into three columns.

The examples compare:

### Border

```text
0px
5px
10px
```

### Margin

```text
0px
5px
10px
```

### Padding

```text
0px
5px
10px
```

The gallery makes it possible to visually compare how changing each property affects an element.

CSS Grid is used to organize the gallery:

```css
.box-gallery {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}
```

---

# CSS Font Units

The project demonstrates six different font-size values using inline styling.

The same text is displayed using different absolute and relative sizing approaches.

## Absolute Units

### Pixels (`px`)

```html
<span style="font-size: 16px;">
    John Paintsil.
</span>
```

Pixels provide a specific screen-based size and may be useful when precise dimensions are needed.

### Points (`pt`)

```html
<span style="font-size: 18pt;">
    John Paintsil.
</span>
```

Points are traditionally associated with printed documents and print-oriented measurements.

---

## Relative Units

### `em`

```html
<span style="font-size: 1em;">
    John Paintsil.
</span>
```

`em` font sizing is relative to the font size inherited from the parent element.

### `rem`

```html
<span style="font-size: 1.25rem;">
    John Paintsil.
</span>
```

`rem` is relative to the font size of the root HTML element.

### Percentage

```html
<span style="font-size: 125%;">
    John Paintsil.
</span>
```

Percentage-based font sizing scales relative to the inherited font size.

### `larger`

```html
<span style="font-size: larger;">
    John Paintsil.
</span>
```

The `larger` keyword instructs the browser to use a font size larger than the inherited size.

---

# CSS Positioning

The project demonstrates four CSS positioning techniques:

1. Relative
2. Absolute
3. Sticky
4. Fixed

---

## Relative Positioning

```css
.position-card {
    position: relative;
}
```

Relative positioning maintains an element's place in the normal document flow while also allowing the element to serve as a positioning reference for absolutely positioned child elements.

A common use case is a card containing a badge or overlay.

---

## Absolute Positioning

```css
.position-badge {
    position: absolute;
    top: 10px;
    right: 10px;
}
```

Absolute positioning allows an element to be positioned at a specific location relative to an appropriate positioned ancestor.

Possible uses include:

- Badges
- Notification counters
- Labels
- Icons
- Overlays

In this project, the absolute element is positioned relative to the `.position-card` element.

---

## Sticky Positioning

```css
.sticky-note {
    position: sticky;
    top: 0;
}
```

Sticky positioning allows an element to behave normally until the user scrolls to a defined position.

It is useful for:

- Navigation elements
- Section headings
- Table headers
- Important notices

---

## Fixed Positioning

The webpage footer uses fixed positioning:

```css
footer {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
}
```

A fixed element remains positioned relative to the browser viewport even while the user scrolls.

In this project, it ensures that the footer remains at the bottom of the screen.

Additional bottom padding is added to the page to prevent the fixed footer from covering content:

```css
body {
    padding-bottom: 70px;
}
```

---

# Running the Project Locally

Because the project is currently a static HTML/CSS website, no build process is required.

## Option 1 — Open Directly

Clone the repository:

```bash
git clone https://github.com/jpaintsil-neu/html-css-javascript.git
```

Enter the project directory:

```bash
cd html-css-javascript
```

Open the project in Visual Studio Code:

```bash
code .
```

Then open:

```text
index.html
```

in a web browser.

---

## Option 2 — VS Code Live Server

For a more convenient development experience, the project can be opened using the VS Code **Live Server** extension.

1. Open the project folder in VS Code.
2. Install the Live Server extension if necessary.
3. Right-click `index.html`.
4. Select **Open with Live Server**.
5. The webpage will open in the default browser.

Live Server automatically refreshes the page after saved changes.

---

# Version Control Workflow

Git is used to track changes locally and synchronize the project with GitHub.

A typical development workflow is:

```bash
git status
git add .
git commit -m "Describe the changes"
git push
```

To retrieve changes from GitHub:

```bash
git pull
```

This allows the local VS Code project and the remote GitHub repository to remain synchronized.

---

# Deployment

The project is deployed using **GitHub Pages**.

GitHub Pages publishes the website directly from the repository's `main` branch.

Deployment configuration:

```text
Source: Deploy from a branch
Branch: main
Folder: / (root)
```

The presence of `index.html` in the root directory allows GitHub Pages to use it as the site's main entry page.

Live website:

**https://jpaintsil-neu.github.io/html-css-javascript/**

---

# Development Workflow

The project followed this general workflow:

```text
Assignment Requirements
        ↓
HTML page structure
        ↓
HTML content and semantic elements
        ↓
SEO research and metadata
        ↓
3 × 3 HTML demonstration
        ↓
CSS box-model gallery
        ↓
Font-unit demonstrations
        ↓
CSS positioning demonstrations
        ↓
Testing in the browser
        ↓
Git version control
        ↓
GitHub repository
        ↓
GitHub Pages deployment
```

---

# Key Learning Outcomes

Through this project, the following concepts were practiced:

- Structuring an HTML5 document
- Understanding `<head>` versus `<body>`
- Creating semantic page sections
- Using IDs for internal navigation
- Understanding block and inline HTML elements
- Using common HTML tags
- Understanding foundational SEO metadata
- Understanding HTML heading hierarchy
- Separating HTML content from CSS presentation
- Understanding the CSS box model
- Comparing margin, border, and padding
- Using absolute and relative CSS units
- Applying inline styling
- Understanding relative positioning
- Understanding absolute positioning
- Understanding sticky positioning
- Understanding fixed positioning
- Using Git for source control
- Synchronizing a VS Code project with GitHub
- Publishing a static website with GitHub Pages

---

# Future Improvements

As CS 5610 progresses, this repository may be expanded to demonstrate additional web-development concepts such as:

- JavaScript fundamentals
- DOM manipulation
- Event handling
- Form validation
- Responsive web design
- CSS Flexbox
- Advanced CSS Grid layouts
- Bootstrap
- Node.js
- Express
- REST APIs
- MongoDB
- React
- Accessibility
- Web security
- Testing

---

# Academic Context

This repository was developed as part of coursework for:

**CS 5610 — Web Development**  
**Northeastern University**

The project is intended to demonstrate understanding of introductory HTML and CSS concepts through implementation and explanation.

---

# Generative AI Disclosure

Generative AI was used as a learning and development aid during this project.

**Tool:** ChatGPT  
**Model:** GPT-5.6 Sol

AI assistance was used to:

- Clarify HTML and CSS concepts
- Interpret assignment requirements
- Review webpage structure
- Explain SEO metadata
- Review HTML and CSS implementation
- Identify issues with IDs and internal navigation
- Explain CSS box-model behavior
- Explain CSS positioning techniques

AI-generated suggestions were reviewed and incorporated as part of the development and learning process.

> Course submissions should include any additional AI-use information required by the instructor, including relevant prompts where applicable.

---

# Author

**John Paintsil**

CS 5610 — Web Development  
Northeastern University

---

## License

This repository was created primarily for educational and academic purposes.

Unless otherwise specified, reuse should respect the course's academic-integrity requirements and applicable source attribution requirements.
