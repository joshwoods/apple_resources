

- AppKit
- NSTextLineFragment
-  attributedString 

Instance Property

# attributedString

The source attributed string.

macOS 12.0+

``` source
var attributedString: NSAttributedString { get }
```

## See Also

### Line fragment characteristics

var characterRange: NSRange

The string range for the source attributed string that corresponds to this line fragment.

var glyphOrigin: CGPoint

Rendering origin for the left-most glyph in the line fragment coordinate system.

var typographicBounds: CGRect

The typographic bounds that specifies the dimensions of the line fragment for laying out line fragments to each other.

