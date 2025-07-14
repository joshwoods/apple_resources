

- Core Text
-  CTFontCreateForStringWithLanguage(\_:\_:\_:\_:) 

Function

# CTFontCreateForStringWithLanguage(\_:\_:\_:\_:)

Returns a font reference that most accurately maps the string range based on the current font and language.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCreateForStringWithLanguage(
    _ currentFont: CTFont,
    _ string: CFString,
    _ range: CFRange,
    _ language: CFString?
) -> CTFont
```

## Parameters 

`currentFont`  

The current font that contains a valid cascade list.

`string`  

A Unicode string containing characters that can’t be encoded by the current font.

`range`  

A CFRange specifying the range of the string to map.

`language`  

A language identifier to select a font for a particular localization.

## Return Value

The best substitute font that can encode the specified string range.

## Discussion

The current font itself can be returned if it covers the string provided. If the caller does not specify the language parameter, the function uses the current system language. The format of the language identifier should conform to UTS #35.

## See Also

### Related Documentation

func CTFontCopyCharacterSet(CTFont) -> CFCharacterSet

Returns the Unicode character set of the font.

func CTFontGetGlyphsForCharacters(CTFont, UnsafePointer&lt;UniChar>, UnsafeMutablePointer&lt;CGGlyph>, CFIndex) -> Bool

Performs basic character-to-glyph mapping.

let kCTFontCascadeListAttribute: CFString

The cascade list used for a font reference.

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

func CTFontCreateCopyWithFamily(CTFont, CGFloat, UnsafePointer&lt;CGAffineTransform>?, CFString) -> CTFont?

Returns a new font in the specified family based on the traits of the original font.

func CTFontCreateForString(CTFont, CFString, CFRange) -> CTFont

Returns a font reference that most accurately maps the string range based on the current font.

