# Web Development Lessons Summary

## 1. HTML Structure and Semantic Elements

- The `<frame>` tag is obsolete and replaced by `<iframe>`.
- Modern HTML emphasizes **semantic tags** such as `<main>`, `<aside>`, `<nav>`, `<footer>`, `<article>`, and `<section>`.
- Semantic HTML helps browsers, search engines, and assistive technologies understand the content better.
- Always use **meaningful variable names** in JavaScript, just as you use semantic tags in HTML.

### Attribute Example ### 

```html

id="greeting"

```

**Format:** `attribute="value"`

### Links

Links can point to:
- The same page (anchors)
- External pages

### Debugging ###

The term **"debug"** comes from the 1960s when an actual insect ("bug") caused a malfunction in an early computer. Debugging means finding and fixing errors in code. Commenting your code helps isolate and resolve issues.

---

## 2. The `<meta>` Tag and Metadata ##

The `<meta>` tag provides **metadata** (data about data) about an HTML page. It is placed inside the `<head>` section and is not visible to users.

### Syntax  ###

```html

<meta name="author" content="John Doe">

```

### Common `<meta>` Attributes and Examples ###

| Attribute             | Example                                                                                       | Description                                           |
|-----------------------|-----------------------------------------------------------------------------------------------|-------------------------------------------------------|
| `charset`             | `<meta charset="UTF-8">`                                                                      | Defines character encoding (UTF-8 recommended).       |
| `name="author"`       | `<meta name="author" content="Jane Smith">`                                                   | Defines the author of the page.                       |
| `name="description"`  | `<meta name="description" content="An introduction to HTML5 and semantic web development.">`  | Short description for SEO.                            |
| `name="keywords"`     | `<meta name="keywords" content="HTML5, CSS, web design, development">`                        | List of keywords (less relevant today for SEO).       |
| `name="viewport"`     | `<meta name="viewport" content="width=device-width, initial-scale=1.0">`                      | Ensures proper rendering on mobile devices.           |
| `name="robots"`       | `<meta name="robots" content="index, follow">`                                                | Tells search engines whether to index the page.       |
| `property="og:title"` | `<meta property="og:title" content="Learn HTML5 Basics">`                                     | Open Graph data (used by Facebook, LinkedIn, etc.).   |
| `property="og:image"` | `<meta property="og:image" content="https://example.com/image.jpg">`                          | Defines preview image for social sharing.             |
| `name="isbn"`         | `<meta name="isbn" content="978-3-16-148410-0">`                                              | Useful for book-related metadata.                     |

### Example with Structured Data (Schema.org) ###

```html

<div itemscope itemtype="http://schema.org/Book">

&nbsp; <span itemprop="name">HTML5: Building Tomorrow's Web Today</span>

&nbsp; <meta itemprop="isbn" content="978-3-16-148410-0">

</div>

```


**Why use `<meta>` tags?**

- **SEO Optimization** – Search engines use metadata to understand page content.
- **Interoperability** – Allows integration with external systems like digital libraries or e-commerce.
- **Accessibility** – Metadata can be used by screen readers or specialized tools.

---

## 3. Schema.org and Open Graph ##

- **Schema.org** adds semantic metadata (for books, events, courses, etc.) to help search engines understand page content.
- Example: adding `itemprop="duration"` or `itemprop="location"` for a course.
- **Open Graph Protocol (OGP)** — created by Facebook, allows control over how a page preview appears when shared on social media (e.g., title, description, image).

---

## 4. Citations and Copyrights ##

- `<cite>` – for short inline quotations.  
- `<blockquote>` – for longer quoted sections (paragraphs).  
- Using these tags signals to search engines that the text is a quotation, preventing SEO penalties for plagiarism.

**Important:** Always credit the original author. Using `<blockquote>` clarifies that you are citing, not copying.

---

## 5. Accessibility (Legge Stanca, 2007 – Italy) ##

From **June 28, 2025**, all websites (public and commercial) must comply with accessibility requirements defined by the **Stanca Law**. Accessibility ensures that visually impaired users can also navigate and interact with websites effectively.

---

## 6. Content and Media Tags ##

- **Content is King** — content quality defines website value.
- HTML provides specific tags for multimedia:
&nbsp; - `<img>` for images
&nbsp; - `<audio>` for sound
&nbsp; - `<video>` for video content
- Other useful formatting tags: `<del>`, `<ins>`, `<strike>`, `<code>`, `<span>`.

---

## 7. SEO, Site Speed, and Tools ##

- Use **PageSpeed Insights** ([https://pagespeed.web.dev](https://pagespeed.web.dev)) to test website performance.
- Example: Spotify optimized its Play button to react within **200ms** for a better user experience.
- Spotify originated from peer-to-peer (P2P) technology.

### Useful Development Resources ###

- [CSS-Tricks](https://css-tricks.com/)
- [HTML.it](https://www.html.it/)
- [MDN Web Docs](https://developer.mozilla.org/)
- [Stack Overflow](https://stackoverflow.com/)
- [FreeCodeCamp](https://www.freecodecamp.org/)

---

## 8. URLs, Domains, and the Wayback Machine ##

### URLs and Domains ###
When purchasing a domain, it is linked to a **server IP address**.
The `/` (slash) indicates the **root directory**.

Example:

```html

<a href="/index.html">Home</a>

```

### Finding a Sitemap ###

1. Try common sitemap URLs:
&nbsp;  - `https://www.labforweb.it/sitemap.xml`
&nbsp;  - `https://www.labforweb.it/sitemap_index.xml`

2. Check `robots.txt` for sitemap links:
&nbsp;  - Example: `Sitemap: https://www.labforweb.it/sitemap.xml`

3. Use tools like **Screaming Frog** or **XML Sitemaps** to find or generate sitemaps.

### The Wayback Machine ###

The **Wayback Machine** ([https://web.archive.org](https://web.archive.org)) by **Internet Archive** allows viewing archived versions of websites from the past.  

It’s useful for research, restoration, and checking old site content.

---

## 9. Key Takeaways ##

- Write **semantic, accessible, and optimized** HTML.
- Always include essential `<meta>` tags for SEO and accessibility.
- Use **Schema.org** and **Open Graph** for structured metadata.
- Test performance, accessibility, and responsiveness.
- Remember: *If you’re not paying for the product, you are the product.*

---

© Compiled from lecture notes on HTML5 and Semantic Web Development.