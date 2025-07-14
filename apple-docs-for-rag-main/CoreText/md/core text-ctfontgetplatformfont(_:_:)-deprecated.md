

- Core Text
-  CTFontGetPlatformFont(\_:\_:) Deprecated

Function

# CTFontGetPlatformFont(\_:\_:)

Returns an ATS font reference and attributes.

macOS 10.5–11.0Deprecated

``` source
func CTFontGetPlatformFont(
    _ font: CTFont,
    _ attributes: UnsafeMutablePointer?>?
) -> ATSFontRef
```

Deprecated

ATS is deprecated

## Parameters 

`font`  

The font reference.

`attributes`  

On output, points to a font descriptor containing additional attributes from the font. Can be `NULL`. Must be released by the caller.

## Return Value

An ATSFontRef object for the given font reference.

## See Also

### Converting Fonts

func CTFontCopyGraphicsFont(CTFont, UnsafeMutablePointer&lt;Unmanaged&lt;CTFontDescriptor>?>?) -> CGFont

Returns a Core Graphics font reference and attributes.

func CTFontCreateWithGraphicsFont(CGFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont

Creates a new font reference from an existing Core Graphics font reference.

func CTFontCreateWithPlatformFont(ATSFontRef, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont?

Creates a new font reference from an ATS font reference.

Deprecated

func CTFontCreateWithQuickdrawInstance(ConstStr255Param?, Int16, UInt8, CGFloat) -> CTFont

Returns a font reference for the given QuickDraw instance.

Deprecated

