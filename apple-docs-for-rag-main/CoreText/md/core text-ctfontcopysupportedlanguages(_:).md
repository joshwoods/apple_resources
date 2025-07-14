

- Core Text
-  CTFontCopySupportedLanguages(\_:) 

Function

# CTFontCopySupportedLanguages(\_:)

Returns an array of languages supported by the font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopySupportedLanguages(_ font: CTFont) -> CFArray
```

## Parameters 

`font`  

The font reference.

## Return Value

A retained reference to an array of languages supported by the font. The array contains language identifier strings as `CFStringRef` objects. The format of the language identifier conforms to the RFC 3066bis standard.

## See Also

### Working With Encoding

func CTFontCopyCharacterSet(CTFont) -> CFCharacterSet

Returns the Unicode character set of the font.

func CTFontGetStringEncoding(CTFont) -> CFStringEncoding

Returns the best string encoding for legacy format support.

