

- AppKit
- NSFont
-  textTransform 

Instance Property

# textTransform

The current transformation matrix of the font.

macOS

``` source
var textTransform: AffineTransform { get }
```

## See Also

### Related Documentation

func set()

Sets this font as the font for the current graphics context.

### Getting the Font Matrices

var matrix: UnsafePointer&lt;CGFloat>

The transformation matrix associated with the font.

class var identityMatrix: UnsafePointer&lt;CGFloat>

The identify matrix for the font.

