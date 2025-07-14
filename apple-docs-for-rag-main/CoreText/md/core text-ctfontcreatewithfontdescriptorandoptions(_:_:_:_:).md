

- Core Text
-  CTFontCreateWithFontDescriptorAndOptions(\_:\_:\_:\_:) 

Function

# CTFontCreateWithFontDescriptorAndOptions(\_:\_:\_:\_:)

Returns a new font reference that best matches the given font descriptor.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCreateWithFontDescriptorAndOptions(
    _ descriptor: CTFontDescriptor,
    _ size: CGFloat,
    _ matrix: UnsafePointer?,
    _ options: CTFontOptions
) -> CTFont
```

## Parameters 

`descriptor`  

A font descriptor containing attributes that specify the requested font.

`size`  

The point size for the font reference. If 0.0 is specified, the default font size of 12.0 is used. This parameter is optional.

`matrix`  

The transformation matrix for the font. In most cases, set this parameter to be `NULL`. If `NULL` is specified, the identity matrix is used. This parameter is optional.

`options`  

Options flags. See CTFontOptions for values. This parameter is optional.

## Return Value

A `CTFontRef` that best matches the attributes provided with the font descriptor.

## Discussion

The size and matrix parameters override any specified in the font descriptor, unless they are unspecified (`0.0` for `size` and `NULL` for `matrix` and `options`). A best match font is always returned, and default values are used for any unspecified.

## See Also

### Creating Fonts

func CTFontCreateWithName(CFString, CGFloat, UnsafePointer&lt;CGAffineTransform>?) -> CTFont

Returns a new font reference for the given name.

func CTFontCreateWithNameAndOptions(CFString, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontOptions) -> CTFont

Returns a new font reference for the given name.

func CTFontCreateWithFontDescriptor(CTFontDescriptor, CGFloat, UnsafePointer&lt;CGAffineTransform>?) -> CTFont

Returns a new font reference that best matches the given font descriptor.

func CTFontCreateUIFontForLanguage(CTFontUIFontType, CGFloat, CFString?) -> CTFont?

Returns the special user-interface font for the given language and user-interface type.

func CTFontCreateCopyWithAttributes(CTFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontDescriptor?) -> CTFont

Returns a new font with additional attributes based on the original font.

func CTFontCreateCopyWithSymbolicTraits(CTFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CTFontSymbolicTraits, CTFontSymbolicTraits) -> CTFont?

Returns a new font in the same font family as the original with the specified symbolic traits.

func CTFontCreateCopyWithFamily(CTFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CFString) -> CTFont?

Returns a new font in the specified family based on the traits of the original font.

func CTFontCreateForString(CTFont, CFString, CFRange) -> CTFont

Returns a font reference that most accurately maps the string range based on the current font.

func CTFontCreateForStringWithLanguage(CTFont, CFString, CFRange, CFString?) -> CTFont

Returns a font reference that most accurately maps the string range based on the current font and language.

