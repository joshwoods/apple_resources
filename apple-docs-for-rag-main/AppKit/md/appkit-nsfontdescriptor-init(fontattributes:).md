

- AppKit
- NSFontDescriptor
-  init(fontAttributes:) 

Initializer

# init(fontAttributes:)

Initializes and returns a new font descriptor with the specified attributes.

macOS

``` source
init(fontAttributes attributes: [NSFontDescriptor.AttributeName : Any]? = nil)
```

## Parameters 

`attributes`  

The attributes for the new font descriptor. If `nil`, the font descriptor’s attribute dictionary will be empty.

## Return Value

The new font descriptor.

## See Also

### Creating a Font Descriptor

class func preferredFontDescriptor(forTextStyle: NSFont.TextStyle, options: [NSFont.TextStyleOptionKey : Any]) -> NSFontDescriptor

Returns a font descriptor that contains the text style.

init(name: String, matrix: AffineTransform)

Returns a font descriptor with the name and matrix attributes set to the given values.

init(name: String, size: CGFloat)

Returns a font descriptor with the name and size attributes set to the given values.

