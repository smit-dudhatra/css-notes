**Question:** I gave my `.parent` element `height: 100%`, but it doesn’t fill the viewport. Why?

**Answer:** `height: 100%` means 100% of the containing parent’s height, not the viewport’s height.

Your HTML structure is:

```text
html → body → .parent
```

Neither `html` nor `body` has an explicit height, so their height depends on their content. As a result, `.parent`’s percentage height behaves like `auto`.

To keep using `height: 100%`, use:

```css
html,
body {
    height: 100%;
}

body {
    margin: 0;
}

.parent {
    display: flex;
    height: 100%;
    border: 2px solid red;
    box-sizing: border-box;
}
```

- `html` and `body` establish the height that `.parent` references.
- `margin: 0` removes the browser’s default body spacing.
- `box-sizing: border-box` includes the border within the specified height.

Alternatively, replace `.parent`’s `height: 100%` with:

```css
min-height: 100vh;
```

`100vh` means 100% of the viewport height, independent of the parent’s explicit height. Using `min-height` also allows the element to grow when its content needs more space. Keep the margin reset and `box-sizing` rule with this approach.
