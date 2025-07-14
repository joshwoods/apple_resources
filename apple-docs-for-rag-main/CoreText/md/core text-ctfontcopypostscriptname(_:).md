

- Core Text
-  CTFontCopyPostScriptName(\_:) 

Function

# CTFontCopyPostScriptName(\_:)

Returns the PostScript name of the given font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyPostScriptName(_ font: CTFont) -> CFString
```

## Parameters 

`font`  

The font reference.

## Return Value

A retained reference to the PostScript name of the font.

## See Also

### Getting Font Names

func CTFontCopyFamilyName(CTFont) -> CFString

Returns the family name of the given font.

func CTFontCopyFullName(CTFont) -> CFString

Returns the full name of the given font.

func CTFontCopyDisplayName(CTFont) -> CFString

Returns the display name of the given font.

func CTFontCopyName(CTFont, CFString) -> CFString?

Returns a reference to the requested name of the given font.

func CTFontCopyLocalizedName(CTFont, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>?) -> CFString?

Returns a reference to a localized name for the given font.

