

- RealityKit
- USD Assets
- USDZ schemas for AR
- Preliminary_Text
-  wrapMode 

Article

# wrapMode

An option that determines the flow of the text.

## Overview

The default value is `flowing`.

### Wrap Modes

`singleLine`  
Displays text in a single line.

`hardBreaks`  
Breaks the text only at the text string’s line breaks.

`flowing`  
Breaks the text as needed to fit within the bounding box.

### Declaration

```
token wrapMode = "flowing" (
    allowedTokens = ["singleLine", "hardBreaks", "flowing"]
)
```

## See Also

### Properties

content

The characters that the text displays.

font

An array of font names.

pointSize

The size of the text’s font.

width

The width of the text’s bounding box.

height

The height of the text’s bounding box.

depth

A value that defines the depth, in scene units, of the text’s extrusion.

horizontalAlignment

An option that controls the text’s horizontal placement within its bounding box.

verticalAlignment

An option that controls the text’s vertical placement within its bounding rectangle.

