# Headers

```md
# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
```

# Bold, Italic, Strikethrough

```md
**Bold**
__Bold__
*Italic*
_italic_
**_Bold_Italic_**
~~Strikethrough~~
```

# Escape command (\\)

```md
\*\*Bold**
```
# Superscript (\^^)(\<sup></sub>) and Subscript (\~~)

```html
X <sup>sup</sup> <!-- Superscript -->
Y <sub>sub</sub> <!-- Subscript -->
```

# Blockquotes

```md
```This text is inside blockquotes.```
```

# Horizontal Rules (---)

```md
-----
*****
_____
```

# Task List ( \- [ ])

```md
- [ ] *Item 1*
- [x] **_Item 2_**
- [ ] ~~Item 3~~
```

# Ordered List

```md
1. Point 1
    1. Subpoint 11
    2. Subpoint 1-2
        - _Details_
2. ~~Striked Point 2~~
3. Point 3
    * __Bold Details__
    * List
        * Item 1
        * Item 2
```

# Unordered List

```md
+ Level 1
  1. Ordered List
     1. Point 1
        - [ ] ~~Ignore~~
        - [ ] Item 1
        - [x] Item 2
     2. Point 2
        * Write your details here
+ Level 2
  + Sublevel 1
    - Points
+ Level 3
```
  
# Tables with alignment

```md
| **Bold Header** | _Italic Header_   | Details |
|:----------------|:-----------------:|--------:|
|_Italic_         |~~Strikethrough~~  |sample   |
```

# Hyperlink

```md
[SLB](https://www.slb.com)
```
# Images (\!\[]())

```md
1. Image
   
    ![Docker](./images/docker.jpg)

2. Clickable image
   
    [![Podman](./images/podman.jfif)](https://podman.io/)
```

# Code block with syntax highlighting(\```)

```md
```ts
import express, { Request, Response } from "express";

// Create a new express application instance
const app = express();

// Set the network port
const port = process.env.PORT || 3000;

// Define the root path with a greeting message
app.get("/", (req: Request, res: Response) => {
    res.json({ message: "Welcome to the Express + TypeScript Server!" });
});

// Start the Express server
app.listen(port, () => {
    console.log(`The server is running at http://localhost:${port}`);
});
```

# Inline HTML Scripting

```html
<h1>Header 1</h1>
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
</ol>
<img src="./images/linux.jfif" width=300 height=300/>
```

# Footnotes (\[^first])

```md
- [Markdown] guide
- [Basic] syntax
- [Extended] syntax

[markdown]: https://www.markdownguide.org/
[basic]: https://www.markdownguide.org/basic-syntax/
[extended]: https://www.markdownguide.org/extended-syntax/
```