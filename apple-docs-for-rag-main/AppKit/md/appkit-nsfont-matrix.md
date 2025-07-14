

- AppKit
- NSFont
-  matrix 

Instance Property

# matrix

The transformation matrix associated with the font.

macOS

``` source
var matrix: UnsafePointer { get }
```

## Discussion

This property contains a standard six-element transformation matrix as used in the PostScript language, specifically with the `makefont` operator. In most cases, with a font of `fontSize`, this matrix is \[`fontSize` 0 0 `fontSize` 0 0\].

## See Also

### Related Documentation

init?(descriptor: NSFontDescriptor, size: CGFloat)

Returns a font object for the specified font descriptor and font size.

### Getting the Font Matrices

var textTransform: AffineTransform

The current transformation matrix of the font.

class var identityMatrix: UnsafePointer&lt;CGFloat>

The identify matrix for the font.

