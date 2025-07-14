

- UIKit
- NSTextLineFragment
-  attributedString 

Instance Property

# attributedString

The source attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

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

