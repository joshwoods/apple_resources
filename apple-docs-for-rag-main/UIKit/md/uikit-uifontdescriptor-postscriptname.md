

- UIKit
- UIFontDescriptor
-  postscriptName 

Instance Property

# postscriptName

The PostScript name of the font descriptor.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var postscriptName: String { get }
```

## See Also

### Querying a font descriptor

var fontAttributes: [UIFontDescriptor.AttributeName : Any]

The font descriptor’s dictionary of attributes.

var matrix: CGAffineTransform

The current transform matrix of the font descriptor.

func object(forKey: UIFontDescriptor.AttributeName) -> Any?

Returns the font attribute that the corresponding key specifies.

var pointSize: CGFloat

The point size of the font descriptor.

var symbolicTraits: UIFontDescriptor.SymbolicTraits

The traits of the font descriptor.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

