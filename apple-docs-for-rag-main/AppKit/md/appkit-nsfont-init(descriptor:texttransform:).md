

- AppKit
- NSFont
-  init(descriptor:textTransform:) 

Initializer

# init(descriptor:textTransform:)

Returns a font object for the specified font descriptor and text transform.

macOS

``` source
init?(
    descriptor fontDescriptor: NSFontDescriptor,
    textTransform: AffineTransform?
)
```

## Parameters 

`fontDescriptor`  

The font descriptor object describing the font to return.

`textTransform`  

An affine transformation applied to the font.

## Return Value

A font object for the specified name and transform.

## Discussion

In most cases, you can simply use init(name:size:) to create standard scaled fonts. If `textTransform` is non-nil, it has precedence over `NSFontMatrixAttribute` in `fontDescriptor`.

## See Also

### Creating Arbitrary Fonts

init?(name: String, size: CGFloat)

Creates a font object for the specified font name and font size.

init?(descriptor: NSFontDescriptor, size: CGFloat)

Returns a font object for the specified font descriptor and font size.

init?(name: String, matrix: UnsafePointer&lt;CGFloat>)

Returns a font object for the specified font name and matrix.

