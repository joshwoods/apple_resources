

- AppKit
- NSFontDescriptor
-  preferredFontDescriptor(forTextStyle:options:) 

Type Method

# preferredFontDescriptor(forTextStyle:options:)

Returns a font descriptor that contains the text style.

macOS 11.0+

``` source
class func preferredFontDescriptor(
    forTextStyle style: NSFont.TextStyle,
    options: [NSFont.TextStyleOptionKey : Any] = [:]
) -> NSFontDescriptor
```

## Parameters 

`style`  

The text style for which to return a font descriptor. See NSFont.TextStyle for available values.

`options`  

A dictionary you use to further configure the returned font descriptor. See NSFont.TextStyleOptionKey for a list of valid keys. Pass an empty dictionary to use the default configuration.

## Return Value

The font descriptor that contains the text style.

## Discussion

The font descriptor contains a dictionary of attributes that you use to create an NSFont object. See NSFontDescriptor for more information.

## See Also

### Creating a Font Descriptor

init(name: String, matrix: AffineTransform)

Returns a font descriptor with the name and matrix attributes set to the given values.

init(name: String, size: CGFloat)

Returns a font descriptor with the name and size attributes set to the given values.

init(fontAttributes: [NSFontDescriptor.AttributeName : Any]?)

Initializes and returns a new font descriptor with the specified attributes.

