

- AppKit
- NSFont
-  renderingMode 

Instance Property

# renderingMode

The rendering mode of the font.

macOS

``` source
var renderingMode: NSFontRenderingMode { get }
```

## Discussion

For a list of valid rendering modes, see NSFontRenderingMode.

## See Also

### Related Documentation

func screenFont(with: NSFontRenderingMode) -> NSFont

Returns a bitmapped screen font, when sent to a font object representing a scalable PostScript font, with the specified rendering mode, matching the receiver in typeface and matrix (or size), or `nil` if such a font can’t be found.

### Instance Properties

var printer: NSFont

The scalable PostScript font corresponding to current font.

var screen: NSFont

The bitmapped screen font for the current font.

