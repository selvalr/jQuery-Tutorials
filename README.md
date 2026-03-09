# jQuery-Tutorials

# jQuery Selectors Guide

This repository contains examples and explanations of **jQuery selectors**.  
Selectors are used to **find and manipulate HTML elements** in the DOM.

---

# 1. Basic Selectors

### `*` (All Selector)
Selects all elements.

```javascript
$("*")
```

Example:
```javascript
$("*").css("color", "blue");
```

---

### `.class`
Select elements by class.

```javascript
$(".box")
```

Example:
```javascript
$(".box").hide();
```

---

### `element`
Select elements by tag name.

```javascript
$("p")
```

Example:
```javascript
$("p").css("color", "red");
```

---

### `#id`
Select element by ID.

```javascript
$("#title")
```

Example:
```javascript
$("#title").text("Hello jQuery");
```

---

### `selector1, selector2`
Select multiple elements.

```javascript
$("h1, p, div")
```

Example:
```javascript
$("h1, p").css("color", "green");
```

---

# 2. Hierarchy Selectors

### `parent > child`
Select direct child elements.

```javascript
$("ul > li")
```

Example:
```javascript
$("div > p").css("color", "blue");
```

---

### `ancestor descendant`
Select all descendant elements.

```javascript
$("div p")
```

Example:
```javascript
$("section p").hide();
```

---

### `prev + next`
Select the next sibling element.

```javascript
$("h1 + p")
```

Example:
```javascript
$("h2 + p").css("color", "red");
```

---

### `prev ~ siblings`
Select all sibling elements after the first element.

```javascript
$("h2 ~ p")
```

Example:
```javascript
$("h2 ~ p").css("background", "yellow");
```

---

# 3. Basic Filters

### `:first`
```javascript
$("p:first")
```

Example:
```javascript
$("p:first").css("color", "blue");
```

---

### `:last`
```javascript
$("p:last")
```

Example:
```javascript
$("p:last").hide();
```

---

### `:eq(index)`
```javascript
$("p:eq(2)")
```

Example:
```javascript
$("li:eq(1)").css("color", "red");
```

---

### `:even`
```javascript
$("li:even")
```

Example:
```javascript
$("li:even").css("background", "lightgray");
```

---

### `:odd`
```javascript
$("li:odd")
```

Example:
```javascript
$("li:odd").css("background", "yellow");
```

---

# 4. Content Filters

### `:contains(text)`
Select elements containing specific text.

```javascript
$("p:contains('hello')")
```

Example:
```javascript
$("p:contains('jQuery')").css("color", "green");
```

---

### `:empty`
Select empty elements.

```javascript
$("div:empty")
```

Example:
```javascript
$("div:empty").remove();
```

---

### `:has(selector)`
Select elements containing another element.

```javascript
$("div:has(p)")
```

Example:
```javascript
$("div:has(img)").css("border", "1px solid red");
```

---

### `:parent`
Select elements that have children.

```javascript
$("div:parent")
```

Example:
```javascript
$("p:parent").css("font-weight", "bold");
```

---

# 5. Visibility Filters

### `:hidden`

```javascript
$("p:hidden")
```

Example:

```javascript
$("p:hidden").show();
```

---

### `:visible`

```javascript
$("p:visible")
```

Example:

```javascript
$("p:visible").css("color", "blue");
```

---

# 6. Attribute Selectors

### `[name]`

```javascript
$("[href]")
```

Example:

```javascript
$("[href]").css("color", "red");
```

---

### `[name="value"]`

```javascript
$("input[type='text']")
```

Example:

```javascript
$("input[type='password']").css("border", "2px solid red");
```

---

### `[name^="value"]` (Starts with)

```javascript
$("a[href^='https']")
```

---

### `[name$="value"]` (Ends with)

```javascript
$("a[href$='.pdf']")
```

---

### `[name*="value"]` (Contains)

```javascript
$("a[href*='google']")
```

---

# 7. Child Filters

### `:first-child`

```javascript
$("li:first-child")
```

Example:

```javascript
$("li:first-child").css("color", "red");
```

---

### `:last-child`

```javascript
$("li:last-child")
```

Example:

```javascript
$("li:last-child").css("color", "blue");
```

---

### `:nth-child(n)`

```javascript
$("li:nth-child(3)")
```

Example:

```javascript
$("li:nth-child(2)").css("background", "yellow");
```

---

### `:only-child`

```javascript
$("p:only-child")
```

Example:

```javascript
$("p:only-child").css("color", "green");
```

---

# Example HTML for Practice

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<p class="box">Hello</p>
<p id="title">Welcome</p>
```

---

# jQuery Setup

Add jQuery to your project:

```html
<script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>
```

---

# Author

Learning jQuery selectors for **frontend development practice**.