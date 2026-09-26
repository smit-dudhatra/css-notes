# CSS Margin Properties

CSS offers several margin properties to control the space **outside an element's border**. These are split into **individual side properties, shorthand properties, and modern logical properties**. [1]

## 1. Individual Side Properties

These properties target a specific physical side of the element: [1]

- `margin-top`: Adds space above the element.
- `margin-right`: Adds space to the right of the element.
- `margin-bottom`: Adds space below the element.
- `margin-left`: Adds space to the left of the element. [2]

## 2. The Shorthand Property (`margin`)

The `margin` property lets you set all four sides in a single line. The behavior changes depending on the number of values you provide: [3, 4]

| Number of Values | Syntax Example | How It Maps to Sides |
| --- | --- | --- |
| **1 Value** | `margin: 10px;` | **All four sides** (Top, Right, Bottom, Left) get 10px. |
| **2 Values** | `margin: 10px 20px;` | First value = **Top & Bottom**; Second value = **Left & Right**. |
| **3 Values** | `margin: 10px 20px 30px;` | First = **Top**; Second = **Left & Right**; Third = **Bottom**. |
| **4 Values** | `margin: 10px 20px 30px 40px;` | Goes clockwise: **Top, Right, Bottom, Left** (TRBL). |

## 3. Logical Properties (Writing-Mode Dependent)

Modern CSS includes logical properties that map to the flow of the text rather than physical screen directions. If your site switches to a right-to-left language (like Arabic), these adapt automatically. [3]

- `margin-block-start`: Top margin in standard horizontal text (start of the block flow). [3]
- `margin-block-end`: Bottom margin in standard horizontal text (end of the block flow). [3]
- `margin-inline-start`: Left margin in standard English text (where the text line starts). [3]
- `margin-inline-end`: Right margin in standard English text (where the text line ends). [3]
- **Shorthands:** `margin-block` (vertical) and `margin-inline` (horizontal). [3]

## Allowed Values

Margin properties accept several types of values: [3]

- **Lengths:** Fixed spacing using units like pixels (`px`), `em`, `rem`, `vh`, or `vw`. [1]
- **Percentages (`%`):** Calculated relative to the **width** of the containing parent element. [1, 5]
- **`auto`:** The browser automatically calculates the margin. For example, combining a fixed width with `margin: 0 auto;` horizontally centers a block element. [1, 2, 3]
- **Negative values:** Using a value like `margin-top: -20px;` pulls adjacent elements closer together or creates overlaps. [3, 6]

Are you trying to **center an element**, space out components in a **grid/flexbox layout**, or troubleshoot a layout issue like **margin collapsing**? Tell me what you are building, and I can provide the exact code you need.

## References

[1] [GeeksforGeeks](https://www.geeksforgeeks.org)

[2] [PBA Institute](https://www.pbainst.in)

[3] [MDN Web Docs](https://developer.mozilla.org)

[4] [Codecademy](https://www.codecademy.com)

[5] [Hyperskill](https://hyperskill.org)

[6] [Scaler](https://www.scaler.com)
