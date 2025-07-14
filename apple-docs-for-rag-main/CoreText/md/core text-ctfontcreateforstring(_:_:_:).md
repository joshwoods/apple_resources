

- Core Text
-  CTFontCreateForString(\_:\_:\_:) 

Function

# CTFontCreateForString(\_:\_:\_:)

Returns a font reference that most accurately maps the string range based on the current font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCreateForString(
    _ currentFont: CTFont,
    _ string: CFString,
    _ range: CFRange
) -> CTFont
```

## Parameters 

`currentFont`  

The current font that contains a valid cascade list.

`string`  

A Unicode string containing characters that can’t be encoded by the current font.

`range`  

A CFRange structure specifying the range of the string to map.

## Return Value

The best substitute font from the cascade list of the current font that can encode the specified string range.

## Discussion

If the current font can encode the string range, the function retains and returns the font.

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

func CTFontCreateForStringWithLanguage(CTFont, CFString, CFRange, CFString?) -> CTFont

Returns a font reference that most accurately maps the string range based on the current font and language.

