

- Core Text
-  CTFontCreateWithGraphicsFont(\_:\_:\_:\_:) 

Function

# CTFontCreateWithGraphicsFont(\_:\_:\_:\_:)

Creates a new font reference from an existing Core Graphics font reference.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCreateWithGraphicsFont(
    _ graphicsFont: CGFont,
    _ size: CGFloat,
    _ matrix: UnsafePointer?,
    _ attributes: CTFontDescriptor?
) -> CTFont
```

## Parameters 

`graphicsFont`  

A valid Core Graphics font reference.

`size`  

The point size for the font reference. If `0.0` is specified the default font size of 12.0 is used.

`matrix`  

The transformation matrix for the font. In most cases, set this parameter to be `NULL`. If `NULL`, the identity matrix is used. Optional.

`attributes`  

Additional attributes that should be matched. Optional.

## Return Value

A new font reference for an existing CGFont object with the specified size, matrix, and additional attributes.

## See Also

### Converting Fonts

func CTFontCopyGraphicsFont(CTFont, UnsafeMutablePointer&lt;Unmanaged&lt;CTFontDescriptor>?>?) -> CGFont

Returns a Core Graphics font reference and attributes.

func CTFontGetPlatformFont(CTFont, UnsafeMutablePointer&lt;Unmanaged&lt;CTFontDescriptor>?>?) -> ATSFontRef

Returns an ATS font reference and attributes.

Deprecated

func CTFontCreateWithPlatformFont(ATSFontRef, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont?

Creates a new font reference from an ATS font reference.

Deprecated

func CTFontCreateWithQuickdrawInstance(ConstStr255Param?, Int16, UInt8, CGFloat) -> CTFont

Returns a font reference for the given QuickDraw instance.

Deprecated

