

- UIKit
- NSTextLineFragment
-  typographicBounds 

Instance Property

# typographicBounds

The typographic bounds that specifies the dimensions of the line fragment for laying out line fragments to each other.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var typographicBounds: CGRect { get }
```

## Discussion

The origin value is offset from the beginning of the line fragment group belonging to the parent layout fragment.

## See Also

### Line fragment characteristics

var attributedString: NSAttributedString

The source attributed string.

var characterRange: NSRange

The string range for the source attributed string that corresponds to this line fragment.

var glyphOrigin: CGPoint

Rendering origin for the left-most glyph in the line fragment coordinate system.

