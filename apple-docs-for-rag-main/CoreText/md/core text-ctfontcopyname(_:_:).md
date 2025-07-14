

- Core Text
-  CTFontCopyName(\_:\_:) 

Function

# CTFontCopyName(\_:\_:)

Returns a reference to the requested name of the given font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyName(
    _ font: CTFont,
    _ nameKey: CFString
) -> CFString?
```

## Parameters 

`font`  

The font reference.

`nameKey`  

The name specifier. See Name Specifier Constants for possible values.

## Return Value

The requested name for the font, or `NULL` if the font does not have an entry for the requested name. The Unicode version of the name is preferred, otherwise the first available version is returned.

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

func CTFontCopyLocalizedName(CTFont, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>?) -> CFString?

Returns a reference to a localized name for the given font.

