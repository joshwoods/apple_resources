

- AppKit
- NSFont
-  init(name:size:) 

Initializer

# init(name:size:)

Creates a font object for the specified font name and font size.

macOS

``` source
init?(
    name fontName: String,
    size fontSize: CGFloat
)
```

## Parameters 

`fontName`  

The fully specified family-face name of the font.

`fontSize`  

The size in points to which the font is scaled.

## Return Value

A font object for the specified name and size.

## Discussion

The value of the `fontName` parameter is a fully specified family-face name, preferably the PostScript name, such as Helvetica-BoldOblique or Times-Roman. (The Font Book app displays PostScript names of fonts in the Font Info panel.)

Specifying `fontSize` is equivalent to using a font matrix of \[`fontSize` 0 0 `fontSize` 0 0\] with init(descriptor:size:). If you use a `fontSize` of 0.0, this method uses the default User Font size.

Fonts created with this method automatically flip themselves in flipped views. This method is the preferred means for creating fonts.

## See Also

### Related Documentation

Cocoa Text Architecture Guide

### Creating Arbitrary Fonts

init?(descriptor: NSFontDescriptor, size: CGFloat)

Returns a font object for the specified font descriptor and font size.

init?(descriptor: NSFontDescriptor, textTransform: AffineTransform?)

Returns a font object for the specified font descriptor and text transform.

init?(name: String, matrix: UnsafePointer&lt;CGFloat>)

Returns a font object for the specified font name and matrix.

