

- Core Text
-  CTFontCopyDefaultCascadeListForLanguages(\_:\_:) 

Function

# CTFontCopyDefaultCascadeListForLanguages(\_:\_:)

Retrieves an ordered list of font substitution preferences.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyDefaultCascadeListForLanguages(
    _ font: CTFont,
    _ languagePrefList: CFArray?
) -> CFArray?
```

## Parameters 

`font`  

The font reference.

`languagePrefList`  

The language preference list, an ordered array of doc://com.apple.documentation/documentation/corefoundation/cfstring-rfhs of ISO language codes.

## Return Value

An ordered list of CTFontDescriptors for font fallback according to the given language preferences.

## Discussion

When the original `font` used for text layout and rendering does not support a certain Unicode character from the provided text, the system follows this list to pick a fallback font that includes the character.

The font alternatives in the cascade list match the original font’s style, weight, and width.

## See Also

### Getting Font Data

func CTFontCopyFontDescriptor(CTFont) -> CTFontDescriptor

Returns the normalized font descriptor for the given font reference.

func CTFontCopyAttribute(CTFont, CFString) -> CFTypeRef?

Returns the value associated with an arbitrary attribute of the given font.

func CTFontGetSize(CTFont) -> CGFloat

Returns the point size of the given font.

func CTFontGetMatrix(CTFont) -> CGAffineTransform

Returns the transformation matrix of the given font.

func CTFontGetSymbolicTraits(CTFont) -> CTFontSymbolicTraits

Returns the symbolic traits of the given font.

func CTFontCopyTraits(CTFont) -> CFDictionary

Returns the traits dictionary of the given font.

