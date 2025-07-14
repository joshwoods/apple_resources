

- Core Text
-  CTFontCreateWithPlatformFont(\_:\_:\_:\_:) Deprecated

Function

# CTFontCreateWithPlatformFont(\_:\_:\_:\_:)

Creates a new font reference from an ATS font reference.

macOS 10.5–11.0Deprecated

``` source
func CTFontCreateWithPlatformFont(
    _ platformFont: ATSFontRef,
    _ size: CGFloat,
    _ matrix: UnsafePointer?,
    _ attributes: CTFontDescriptor?
) -> CTFont?
```

Deprecated

ATS is deprecated

## Parameters 

`platformFont`  

A valid ATSFontRef object.

`size`  

The point size for the font reference. If `0.0` is specified the default font size of 12.0 is used.

`matrix`  

The transformation matrix for the font. In most cases, set this parameter to be `NULL`. If `NULL`, the identity matrix is used. Optional.

`attributes`  

A CTFontDescriptor containing additional attributes that should be matched. Optional.

## Return Value

A new font reference for an ATSFontRef with the specified size, matrix, and additional attributes.

## See Also

### Converting Fonts

func CTFontCopyGraphicsFont(CTFont, UnsafeMutablePointer&lt;Unmanaged&lt;CTFontDescriptor>?>?) -> CGFont

Returns a Core Graphics font reference and attributes.

func CTFontCreateWithGraphicsFont(CGFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont

Creates a new font reference from an existing Core Graphics font reference.

func CTFontGetPlatformFont(CTFont, UnsafeMutablePointer&lt;Unmanaged&lt;CTFontDescriptor>?>?) -> ATSFontRef

Returns an ATS font reference and attributes.

Deprecated

func CTFontCreateWithQuickdrawInstance(ConstStr255Param?, Int16, UInt8, CGFloat) -> CTFont

Returns a font reference for the given QuickDraw instance.

Deprecated

