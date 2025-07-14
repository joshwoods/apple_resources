

- Core Text
-  CTFontCopyGraphicsFont(\_:\_:) 

Function

# CTFontCopyGraphicsFont(\_:\_:)

Returns a Core Graphics font reference and attributes.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyGraphicsFont(
    _ font: CTFont,
    _ attributes: UnsafeMutablePointer?>?
) -> CGFont
```

## Parameters 

`font`  

The font reference.

`attributes`  

On output, points to a font descriptor containing additional attributes from the font. Can be `NULL`. Must be released by the caller.

## Return Value

A CGFont object for the given font reference.

## See Also

### Converting Fonts

func CTFontCreateWithGraphicsFont(CGFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont

Creates a new font reference from an existing Core Graphics font reference.

func CTFontGetPlatformFont(CTFont, UnsafeMutablePointer&lt;Unmanaged&lt;CTFontDescriptor>?>?) -> ATSFontRef

Returns an ATS font reference and attributes.

Deprecated

func CTFontCreateWithPlatformFont(ATSFontRef, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont?

Creates a new font reference from an ATS font reference.

Deprecated

func CTFontCreateWithQuickdrawInstance(ConstStr255Param?, Int16, UInt8, CGFloat) -> CTFont

Returns a font reference for the given QuickDraw instance.

Deprecated

