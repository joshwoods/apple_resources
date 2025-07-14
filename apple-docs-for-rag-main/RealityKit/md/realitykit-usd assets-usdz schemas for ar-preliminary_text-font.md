

- RealityKit
- USD Assets
- USDZ schemas for AR
- Preliminary_Text
-  font 

Article

# font

An array of font names.

## Overview

The runtime scans this list in ascending order and chooses the first font that the runtime can provide. Font names provide the font family, then the font style, such as “Gill Sans.” You can reference font names using Font Book on macOS.

If the system doesn’t support your chosen font, you can fall back to a generic font by providing one or more generic font specifiers at the end of the font list: `serif`, `san-serif`, `monospaced`, or `cursive`.

### Declaration

```
string[] font
```

## See Also

### Properties

content

The characters that the text displays.

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

horizontalAlignment

An option that controls the text’s horizontal placement within its bounding box.

verticalAlignment

An option that controls the text’s vertical placement within its bounding rectangle.

