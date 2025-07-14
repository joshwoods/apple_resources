

- AppKit
- NSFont
-  init(name:matrix:) 

Initializer

# init(name:matrix:)

Returns a font object for the specified font name and matrix.

macOS

``` source
init?(
    name fontName: String,
    matrix fontMatrix: UnsafePointer
)
```

## Parameters 

`fontName`  

The fully specified family-face name of the font.

`fontMatrix`  

A transformation matrix applied to the font.

## Return Value

A font object for the specified name and transformation matrix.

## Discussion

The `fontName` is a fully specified family-face name, such as Helvetica-BoldOblique or Times-Roman (not a name as shown in the Font Panel). The `fontMatrix` is a standard 6-element transformation matrix as used in the PostScript language, specifically with the `makefont` operator. In most cases, you can simply use init(name:size:) to create standard scaled fonts.

You can use the defined value `NSFontIdentityMatrix` for \[1 0 0 1 0 0\]. Fonts created with a matrix other than `NSFontIdentityMatrix` don’t automatically flip themselves in flipped views.

## See Also

### Related Documentation

var isFlipped: Bool

A Boolean value indicating whether the view uses a flipped coordinate system.

### Creating Arbitrary Fonts

init?(name: String, size: CGFloat)

Creates a font object for the specified font name and font size.

init?(descriptor: NSFontDescriptor, size: CGFloat)

Returns a font object for the specified font descriptor and font size.

init?(descriptor: NSFontDescriptor, textTransform: AffineTransform?)

Returns a font object for the specified font descriptor and text transform.

