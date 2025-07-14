

- AppKit
- NSFont
-  printer 

Instance Property

# printer

The scalable PostScript font corresponding to current font.

macOS

``` source
@NSCopying
var printer: NSFont { get }
```

## Discussion

For a font that already represents a scalable PostScript font, the value in this property is `self`. For a bitmapped screen font, the value is the corresponding scalable PostScript font.

## See Also

### Instance Properties

var renderingMode: NSFontRenderingMode

The rendering mode of the font.

var screen: NSFont

The bitmapped screen font for the current font.

