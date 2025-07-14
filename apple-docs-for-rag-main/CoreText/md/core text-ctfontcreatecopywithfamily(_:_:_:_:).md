

- Core Text
-  CTFontCreateCopyWithFamily(\_:\_:\_:\_:) 

Function

# CTFontCreateCopyWithFamily(\_:\_:\_:\_:)

Returns a new font in the specified family based on the traits of the original font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCreateCopyWithFamily(
    _ font: CTFont,
    _ size: CGFloat,
    _ matrix: UnsafePointer?,
    _ family: CFString
) -> CTFont?
```

## Parameters 

`font`  

The original font reference on which to base the new font.

`size`  

The point size for the font reference. If `0.0` is specified, the original font’s size is preserved.

`matrix`  

The transformation matrix for the font. In most cases, set this parameter to be `NULL`. If `NULL` is specified, the original font’s matrix is preserved.

`family`  

The name of the desired family.

## Return Value

A new font reference with the original traits in the given family, or `NULL` if none is found in the system.

## See Also

### Creating Fonts

func CTFontCreateWithName(CFString, CGFloat, UnsafePointer&lt;CGAffineTransform>?) -> CTFont

Returns a new font reference for the given name.

func CTFontCreateWithNameAndOptions(CFString, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontOptions) -> CTFont

Returns a new font reference for the given name.

func CTFontCreateWithFontDescriptor(CTFontDescriptor, CGFloat, UnsafePointer&lt;CGAffineTransform>?) -> CTFont

Returns a new font reference that best matches the given font descriptor.

func CTFontCreateWithFontDescriptorAndOptions(CTFontDescriptor, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontOptions) -> CTFont

Returns a new font reference that best matches the given font descriptor.

func CTFontCreateUIFontForLanguage(CTFontUIFontType, CGFloat, CFString?) -> CTFont?

Returns the special user-interface font for the given language and user-interface type.

func CTFontCreateCopyWithAttributes(CTFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont

Returns a new font with additional attributes based on the original font.

func CTFontCreateCopyWithSymbolicTraits(CTFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontSymbolicTraits, CTFontSymbolicTraits) -> CTFont?

Returns a new font in the same font family as the original with the specified symbolic traits.

func CTFontCreateForString(CTFont, CFString, CFRange) -> CTFont

Returns a font reference that most accurately maps the string range based on the current font.

func CTFontCreateForStringWithLanguage(CTFont, CFString, CFRange, CFString?) -> CTFont

Returns a font reference that most accurately maps the string range based on the current font and language.

