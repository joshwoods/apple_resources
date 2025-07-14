

- AppKit
- NSFontDescriptor
-  init(name:size:) 

Initializer

# init(name:size:)

Returns a font descriptor with the name and size attributes set to the given values.

macOS

``` source
init(
    name fontName: String,
    size: CGFloat
)
```

## Parameters 

`fontName`  

The value for `NSFontNameAttribute`.

`size`  

The value for `NSFontSizeAttribute`.

## Return Value

The new font descriptor.

## See Also

### Creating a Font Descriptor

class func preferredFontDescriptor(forTextStyle: NSFont.TextStyle, options: [NSFont.TextStyleOptionKey : Any]) -> NSFontDescriptor

Returns a font descriptor that contains the text style.

init(name: String, matrix: AffineTransform)

Returns a font descriptor with the name and matrix attributes set to the given values.

init(fontAttributes: [NSFontDescriptor.AttributeName : Any]?)

Initializes and returns a new font descriptor with the specified attributes.

