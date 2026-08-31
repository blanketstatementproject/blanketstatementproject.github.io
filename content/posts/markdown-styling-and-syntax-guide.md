---
title: "Hugo Markdown Styling & Formatting Guide"
date: 2026-03-01T12:00:00-05:00
draft: false
description: "A comprehensive showcase of typography, code highlighting, tables, quotes, and media formatting available in this Hugo blog starter."
image: "img/knitted-squares.jpg"
categories: ["Tutorials", "Tech"]
tags: ["hugo", "markdown", "guide", "starter"]
author: "Blanket Statement Team"
---

This starter template includes rich formatting support for technical writing, tutorial posts, and personal blogging. Below is a preview of the typography and components.

## Headings & Typography

Here is standard body text with **bold text**, *italic text*, and `inline code`.

### Subheading Level 3

Paragraph text flows smoothly with readable line heights and carefully tuned margins matching the Blanket Statement visual identity.

#### Subheading Level 4

Lists are formatted with clean spacing:

* First bullet point with helpful context
* Second bullet point with [a link to home](/)
* Third bullet point with embedded sub-items:
  * Sub-item A
  * Sub-item B

## Blockquotes

> "Productive fidgeting transforms passive listening into active, engaged presence while building something beautiful for others."

## Code Syntax Highlighting

Hugo's built-in Chroma syntax engine formats code with high contrast:

```python
def knit_square(stitches=30, rows=48):
    """Simulate knitting a 7x9 inch square."""
    fabric = []
    for r in range(rows):
        fabric.append(["knit" for _ in range(stitches)])
    print(f"Finished square with {rows} rows of {stitches} stitches!")
    return fabric

if __name__ == "__main__":
    knit_square()
```

And in Go / Hugo template syntax:

```go
{{ range where .Site.RegularPages "Section" "posts" }}
  <article>
    <h2>{{ .Title }}</h2>
    <p>{{ .Summary }}</p>
  </article>
{{ end }}
```

## Tables

| Metric | Target | Notes |
| :--- | :--- | :--- |
| **Block Width** | 7 inches | Standard size |
| **Block Length** | 9 inches | Direction doesn't matter |
| **Yarn Weight** | Worsted (#4) | Washable acrylic or wool blend |
| **Needle Size** | US 8 (5.0mm) | Provides flexible drape |

## Image Embeds

Images are automatically responsive with rounded corners and subtle shadows:

![Knitting with colorful yarn](/img/balls-of-yarn.jpg)

Enjoy writing your posts with Hugo!
