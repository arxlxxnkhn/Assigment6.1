## Assignment 6.1 — Box Model Inspection

### 1. `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS Box Model</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>CSS Box Model</h1>

    <div class="box box1">
        <h2>Box 1</h2>
        <p>Content-box example.</p>
    </div>

    <div class="box box2">
        <h2>Box 2</h2>
        <p>Border-box example.</p>
    </div>

    <div class="box box3">
        <h2>Box 3</h2>
        <p>Different padding, border, and margin.</p>
    </div>
</body>
</html>
```

### 2. `style.css`

```css
.box {
    width: 300px;
    background: lightblue;
}

.box1 {
    box-sizing: content-box;
    padding: 20px;
    border: 5px solid navy;
    margin: 15px;
}

.box2 {
    box-sizing: border-box;
    padding: 20px;
    border: 5px solid green;
    margin: 25px;
}

.box3 {
    box-sizing: border-box;
    padding: 30px;
    border: 8px dashed red;
    margin: 35px;
}
```

### 3. Box Model Explanation

- **Content:** The text or actual content inside the element.
- **Padding:** Space between content and border.
- **Border:** Line surrounding the padding and content.
- **Margin:** Space outside the border.

**Difference:** `content-box` adds padding and border to the specified width. `border-box` includes padding and border within the specified width.

**Submission:** Open the page in Chrome, press `F12`, select an element, and inspect the **Box Model** diagram. Take a screenshot and label content, padding, border, and margin.