

- AppKit
- NSFontDescriptor
-  init(name:matrix:) 

Initializer

# init(name:matrix:)

Returns a font descriptor with the name and matrix attributes set to the given values.

macOS

``` source
init(
    name fontName: String,
    matrix: AffineTransform
)
```

## Parameters 

`fontName`  

The value for `NSFontNameAttribute`.

`matrix`  

The value for `NSFontMatrixAttribute`.

## Return Value

The new font descriptor.

## See Also

### Creating a Font Descriptor

class func preferredFontDescriptor(forTextStyle: NSFont.TextStyle, options: [NSFont.TextStyleOptionKey : Any]) -> NSFontDescriptor

Returns a font descriptor that contains the text style.

init(name: String, size: CGFloat)

Returns a font descriptor with the name and size attributes set to the given values.

init(fontAttributes: [NSFontDescriptor.AttributeName : Any]?)

Initializes and returns a new font descriptor with the specified attributes.

