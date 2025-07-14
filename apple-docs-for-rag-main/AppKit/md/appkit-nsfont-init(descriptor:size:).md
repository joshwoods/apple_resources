

- AppKit
- NSFont
-  init(descriptor:size:) 

Initializer

# init(descriptor:size:)

Returns a font object for the specified font descriptor and font size.

macOS

``` source
init?(
    descriptor fontDescriptor: NSFontDescriptor,
    size fontSize: CGFloat
)
```

## Parameters 

`fontDescriptor`  

A font descriptor object.

`fontSize`  

The size in points to which the font is scaled.

## Return Value

A font object for the specified descriptor and size.

## Discussion

In most cases, you can simply use init(name:size:) to create standard scaled fonts.

## See Also

### Creating Arbitrary Fonts

init?(name: String, size: CGFloat)

Creates a font object for the specified font name and font size.

init?(descriptor: NSFontDescriptor, textTransform: AffineTransform?)

Returns a font object for the specified font descriptor and text transform.

init?(name: String, matrix: UnsafePointer&lt;CGFloat>)

Returns a font object for the specified font name and matrix.

