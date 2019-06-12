# Training Kit

## Data attributes

> Data attributes gives devs another way to hook into the DOM without having to use classes and IDs as a unique way to make selections

### Overview

HTML5 allows us to make our own attributes using the `data-` prefix

```html
<div data-school="Lambda" class="school">Lambda School</div>
```

```css
div[data-school="Lambda"] {
  /* styles */
}
```

To acces in JS, use .dataset property - returns an object that we can access using dot notation

```js
const school = document.querySelector(".school");
const schoolName = school.dataset.school;
console.log(schoolName); // Lambda
```

Use the data attribute in a CSS style selector

```js
const schoolElement = document.querySelector("div[data-school='Lambda']");
```
