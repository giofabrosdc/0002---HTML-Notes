```markdown
# ⚪ HTML ACCESSIBILITY REVIEW GUIDE ⚫

> **Core Philosophy:** Designing digital spaces that everyone can perceive, operate, understand, and navigate reliably. 

---

## ⚪ 1. Introduction to Accessibility

* **Web Content Accessibility Guidelines (WCAG):** Essential international guidelines for digital inclusion.
* **The POUR Principles:**
  * ⚪ **P**erceivable — Information must be sensible to users.
  * ⚫ **O**perable — Components and navigation must function cleanly.
  * ⚪ **U**nderstandable — Interface and text must be clear.
  * ⚫ **R**obust — Content must adapt to diverse assistive tools.

---

## ⚫ 2. Assistive Technology for Accessibility

* **⚪ Screen Readers:** Audio tools reading screens aloud for blind/low-vision users.
* **⚫ Large Text or Braille Keyboards:** Tactile hardware inputs for visual impairments.
* **⚪ Screen Magnifiers:** Enlargement tools for low-vision navigation.
* **⚫ Alternative Pointing Devices:** Joysticks, trackballs, and touchpads for mobility constraints.
* **⚪ Voice Recognition:** Vocal-command systems enabling hands-free computer control.

---

## ⚪ 3. Accessibility Auditing Tools

* **Common Tools:** 
  * ⚪ Google Lighthouse
  * ⚫ Wave
  * ⚪ IBM Equal Accessibility Checker
  * ⚫ axe DevTools

---

## ⚫ 4. Accessibility Best Practices

* **Proper Heading Structure:** Build a clear, hierarchical outline (`<h1>` through `<h6>`) to give assistive tech proper context.
* **Accessibility and Tables:** 
  * Use `<th>` for headers and `<td>` for data cells.
  * Insert a `<caption>` element *immediately* after the opening `<table>` tag so screen readers announce context first.
* **Input Labels:** Use `<label>` paired with matching `for` and `id` attributes for every input.
* **Span Elements:** A generic inline container used for text styling or anchoring IDs for ARIA references.
* **Good Alt Text:** Provide concise alternative text via `alt` attributes on images.
* **Descriptive Link Text:** Avoid vague phrases; make link destinations crystal clear.
* **Audio & Video Content:** Add captions, transcripts, and audio descriptions for sensory impairments.
* **The `tabindex` Attribute:** Manages keyboard focus order. *Rule:* Never use values greater than `0`. Stick to `0` or `-1`.
  ```html
  <p tabindex="-1">Sorry, there was an error with your submission.</p>

```

* **The `accesskey` Attribute:** Defines quick keyboard navigation shortcuts.
```html
<button accesskey="s">Save</button>
<button accesskey="c">Cancel</button>
<a href="index.html" accesskey="h">Home</a>

```



---

## ⚪ 5. WAI-ARIA, Roles, and Attributes

* **WAI-ARIA:** Accessible Rich Internet Applications attributes added to elements to bridge semantic context gaps.
* **ARIA Roles:** Predefined attributes defining an element's structural purpose.

### ⚫ The Six ARIA Role Categories

1. **Document structure roles:** Define overall page architecture.
2. **Widget roles:** Establish interactive element properties (e.g., scrollbars).
3. **Landmark roles:** Map primary sections for fast screen reader navigation.
4. **Live region roles:** Announce dynamically changing content updates.
5. **Window roles:** Manage modals, dialogues, and alert popups (`dialog`, `alertdialog`).
6. **Abstract roles:** Internal browser use only (do not use in code).

### ⚪ Essential ARIA Attributes in Action

#### ⚪ Accessible Names (`aria-label` & `aria-labelledby`)

```html
<button aria-label="Search">
    <i class="fas fa-search"></i>
</button>
<input type="text" aria-labelledby="search-btn">
<button type="button" id="search-btn">Search</button>

```

#### ⚫ Visual Hiding (`aria-hidden`)

```html
<button>
    <i class="fa-solid fa-gear" aria-hidden="true"></i>
    <span class="label">Settings</span>
</button>

```

#### ⚪ Contextual Associations (`aria-describedby`)

```html
<form>
    <label for="password">Password:</label>
    <input type="password" id="password" aria-describedby="password-help" />
    <p id="password-help">Your password must be at least 8 characters long.</p>
</form>

```

```

```
