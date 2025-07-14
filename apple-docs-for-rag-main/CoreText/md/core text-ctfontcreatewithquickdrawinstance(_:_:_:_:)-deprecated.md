

- Core Text
-  CTFontCreateWithQuickdrawInstance(\_:\_:\_:\_:) Deprecated

Function

# CTFontCreateWithQuickdrawInstance(\_:\_:\_:\_:)

Returns a font reference for the given QuickDraw instance.

macOS 10.5–10.15Deprecated

``` source
func CTFontCreateWithQuickdrawInstance(
    _ name: ConstStr255Param?,
    _ identifier: Int16,
    _ style: UInt8,
    _ size: CGFloat
) -> CTFont
```

Deprecated

Quickdraw font references are deprecated

## Parameters 

`name`  

The QuickDraw font name. If zero length, `identifier` must be specified.

`identifier`  

The QuickDraw font identifier. Can be `0`, but if so, `name` must be specified.

`style`  

The QuickDraw font style.

`size`  

The point size for the font reference. If `0.0` is specified, the default size of 12.0 is used.

## Return Value

The best font instance matching the QuickDraw instance information.

## Discussion

This function is provided for compatibility support between Core Text and clients needing to support QuickDraw-style font references. QuickDraw is a deprecated technology in macOS 10.4 and later.

## See Also

### Converting Fonts

func CTFontCopyGraphicsFont(CTFont, UnsafeMutablePointer&lt;Unmanaged&lt;CTFontDescriptor>?>?) -> CGFont

Returns a Core Graphics font reference and attributes.

func CTFontCreateWithGraphicsFont(CGFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont

Creates a new font reference from an existing Core Graphics font reference.

func CTFontGetPlatformFont(CTFont, UnsafeMutablePointer&lt;Unmanaged&lt;CTFontDescriptor>?>?) -> ATSFontRef

Returns an ATS font reference and attributes.

Deprecated

func CTFontCreateWithPlatformFont(ATSFontRef, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont?

Creates a new font reference from an ATS font reference.

Deprecated

