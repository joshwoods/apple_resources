

- RealityKit
- USD Assets
- USDZ schemas for AR
- Preliminary_Text
-  horizontalAlignment 

Article

# horizontalAlignment

An option that controls the text’s horizontal placement within its bounding box.

## Overview

The default value is `center`.

### Horizontal Alignments

`left`  
Left-aligns each line of text.

`center`  
Center-aligns each line of text.

`right`  
Right-aligns each line of text.

`justified`  
Left- and right-aligns the text by adding additional spaces between words.

### Declaration

```
token horizontalAlignment = "center" (
    allowedTokens = ["left", "center", "right", "justified"]
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

wrapMode

An option that determines the flow of the text.

verticalAlignment

An option that controls the text’s vertical placement within its bounding rectangle.

