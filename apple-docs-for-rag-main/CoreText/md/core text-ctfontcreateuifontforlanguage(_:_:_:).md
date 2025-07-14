

- Core Text
-  CTFontCreateUIFontForLanguage(\_:\_:\_:) 

Function

# CTFontCreateUIFontForLanguage(\_:\_:\_:)

Returns the special user-interface font for the given language and user-interface type.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCreateUIFontForLanguage(
    _ uiType: CTFontUIFontType,
    _ size: CGFloat,
    _ language: CFString?
) -> CTFont?
```

## Parameters 

`uiType`  

A constant specifying the intended user-interface use for the requested font reference. See Enumerations for possible values.

`size`  

The point size for the font reference. If `0.0` is specified, the default size for the requested user-interface type is used.

`language`  

Language specifier string to select a font for a particular localization. If `NULL` is specified, the current system language is used. The format of the language identifier should conform to the RFC 3066bis standard.

## Return Value

The correct font for various user-interface uses.

## Discussion

The only required parameter is the `uiType` selector; the other parameters have default values.

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

