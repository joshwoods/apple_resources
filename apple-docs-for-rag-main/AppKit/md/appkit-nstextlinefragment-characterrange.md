

- AppKit
- NSTextLineFragment
-  characterRange 

Instance Property

# characterRange

The string range for the source attributed string that corresponds to this line fragment.

macOS 12.0+

``` source
var characterRange: NSRange { get }
```

## See Also

### Line fragment characteristics

var attributedString: NSAttributedString

The source attributed string.

var glyphOrigin: CGPoint

Rendering origin for the left-most glyph in the line fragment coordinate system.

var typographicBounds: CGRect

The typographic bounds that specifies the dimensions of the line fragment for laying out line fragments to each other.

