# ⚪ HTML PREP EXAM REVIEW GUIDE ⚫

> **Core Focus:** Comprehensive preparation for your HTML concepts prep exam, formatted cleanly with high-contrast elements.

---

## ⚪ 1. HTML BASICS & STRUCTURE

* **Role of HTML:** Hypertext Markup Language defines the core foundation and structure of a webpage.
* **HTML Elements:** Represent page content, typically enclosed using an opening and closing tag (e.g., `<h1></h1>`, `<p></p>`).
* **HTML Structure & Boilerplate:** Every document begins with a boilerplate containing the DOCTYPE, `<html>`, `<head>` (metadata/styles), and `<body>` (content), utilizing **UTF-8 character encoding** for universal display.
* **Common Elements & Containers:** 
  * Headings (`<h1>` through `<h6>`) and Paragraphs (`<p>`).
  * `<div>`: A generic inline/block container with no semantic meaning used for grouping.
* **Void Elements:** Tags that do not have a closing tag (e.g., `<img>`).
* **Attributes:** Used to add metadata and alter behavior across elements.
* **Identifiers & Grouping:** 
  * **IDs (`id`):** Unique identifiers for a single element.
  * **Classes (`class`):** Reusable groups for shared styling and behavior.

---

## ⚫ 2. SPECIAL CHARACTERS, LINKS & PATHS

* **HTML Entities:** Rendering special symbols safely (e.g., `&amp;`, `&lt;`).
* **External Assets:** `<link>` element for external stylesheets; `<script>` for embedding JavaScript files.
* **Paths & Navigation:**
  * **Absolute vs. Relative Paths:** Navigating directories using precise absolute URLs or relative directory notation (`/`, `./`, `../`).
  * **Target Attributes:** Controlling how and where links open.
  * **Link States & Internal Links:** Managing interaction states (hover, active) and jumping to page sections using `href="#id"` coupled with a matching destination `id`.

---

## ⚪ 3. SEO, SOCIAL SHARING & MEDIA OPTIMIZATION

* **SEO & Social Meta Tags:** 
  * Description meta tags summarize page content for search engines.
  * Open Graph tags optimize social media content sharing cards.
* **Media & Replaced Elements:** Embedded content like images and `<iframe>` integrations.
* **Optimization & Formats:** Performance techniques, licensing rules, image formats, and **SVGs (Scalable Vector Graphics)** for crisp vector scaling.
* **Multimedia:** Native HTML `<audio>` and `<video>` tags.

---

## ⚫ 4. SEMANTIC HTML & TEXT FORMATTING

* **Structural Hierarchy:** Maintaining logical heading levels (`<h1>` is highest, `<h6>` is lowest). Avoid presentational tags (like deprecated `<center>`, `<font>`).
* **Semantic Structure Elements:**
  * `<header>`: Introductory content blocks.
  * `<nav>`: Core navigation link collections.
  * `<article>`: Self-contained, independent content.
  * `<aside>`: Sidebars or supplementary information.
  * `<section>`: Thematic grouping of content.
  * `<footer>`: Footer metadata or section closure.
* **Inline Semantics & Text Elements:**
  * **Emphasis/Strong:** `<em>` (stress emphasis) and `<strong>` (strong importance).
  * **Idiomatic/Attention:** `<i>` (alternate voice/technical terms) and `<b>` (attention without extra importance).
  * **Quotes & References:** `<q>` (inline), `<blockquote>` (block section), `<abbr>` (abbreviations).
  * **Lists & Metadata:** `<dl>`, `<dt>`, `<dd>` (description lists), `<address>`, `<time>`.
  * **Sub/Sup & Code:** `<sup>`, `<sub>`, `<code>`.
  * **Annotations & Alterations:** `<u>` (unarticulated annotation), `<ruby>` (ruby text), `<s>` (strikethrough for outdated relevance).

---

## ⚪ 5. HTML FORMS, INPUTS & TABLES

### 📋 Form Elements
* **`<form>` Attributes:** `action` (target destination URL) and `method` (`GET` or `POST`).
* **Inputs & Attributes:** 
  * Common types: `text`, `email`, `password`, `radio`, `checkbox`, `number`, `date`.
  * Core attributes: `name` (submission key/radio grouping), `value`, `placeholder`, `size`, `min`, `max`, `minlength`, `maxlength`, `required`, `disabled`, `readonly`.
* **Labels & Association:** 
  * **Implicit:** Wrapping input inside `<label>`.
  * **Explicit:** Using `for="id"` on the label pointing to the input's `id`.
* **Buttons & Grouping:** 
  * `<button>` with types (`submit`, `reset`, `button`).
  * `<fieldset>` and `<legend>` for grouping related controls (like radio or checkbox sets).

### 📊 Table Elements
* Built using `<table>`, `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`, `<tr>`, `<th>` (headers), and `<td>` (data cells).
* **`colspan`:** Controls column spanning across table cells.

---

## ⚫ 6. HTML TOOLS & ACCESSIBILITY (A11Y)

### 🛠️ Developer & Validation Tools
* **HTML Validator:** Checks syntax correctness.
* **DOM Inspector / DevTools:** Browser-native panels to inspect, debug, and profile code.

### 🌐 Introduction to Accessibility
* **WCAG & POUR Principles:** Web Content Accessibility Guidelines broken into **P**erceivable, **O**perable, **U**nderstandable, and **R**obust.
* **Assistive Tech:** Screen readers, braille keyboards, screen magnifiers, alternative pointing devices, and voice recognition systems.
* **Auditing Tools:** Google Lighthouse, WAVE, IBM Equal Accessibility Checker, and axe DevTools.

### 📝 Accessibility Best Practices
* Use correct heading structures and meaningful alt text on images.
* Always bind inputs to descriptive `<label>` elements.
* Provide transcripts, captions, and audio descriptions for multimedia.
* Use `tabindex` strictly as `0` or `-1` (never positive values) and `accesskey` for shortcuts.

### 🏷️ WAI-ARIA, Roles & Attributes
* **ARIA Roles:** Predefined structural functions (e.g., `role="tab"`).
* **Key Attributes:**
  * `aria-label` / `aria-labelledby`: Programmatic accessible names.
  * `aria-hidden`: Hides decorative elements from assistive tools.
  * `aria-describedby`: Links extra helper text, requirements, or error feedback to form inputs.
