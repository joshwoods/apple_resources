

- Core Text
-  CTFontCopyLocalizedName(\_:\_:\_:) 

Function

# CTFontCopyLocalizedName(\_:\_:\_:)

Returns a reference to a localized name for the given font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyLocalizedName(
    _ font: CTFont,
    _ nameKey: CFString,
    _ actualLanguage: UnsafeMutablePointer?>?
) -> CFString?
```

## Parameters 

`font`  

The font reference.

`nameKey`  

The name specifier. See Name Specifier Constants for possible values.

`actualLanguage`  

On output, points to the language string of the returned name string. The format of the language identifier conforms to the RFC 3066bis standard.

## Return Value

A specific localized name from the font reference or `NULL` if the font does not have an entry for the requested name key.

## Discussion

The name is localized based on the user’s global language preference precedence. That is, the user’s language preference is a list of languages in order of precedence. So, for example, if the list had Japanese and English, in that order, then a font that did not have Japanese name strings but had English strings would return the English strings.

## See Also

### Getting Font Names

func CTFontCopyPostScriptName(CTFont) -> CFString

Returns the PostScript name of the given font.

func CTFontCopyFamilyName(CTFont) -> CFString

Returns the family name of the given font.

func CTFontCopyFullName(CTFont) -> CFString

Returns the full name of the given font.

func CTFontCopyDisplayName(CTFont) -> CFString

Returns the display name of the given font.

func CTFontCopyName(CTFont, CFString) -> CFString?

Returns a reference to the requested name of the given font.

