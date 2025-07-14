

- Core Text
-  CTFontGetStringEncoding(\_:) 

Function

# CTFontGetStringEncoding(\_:)

Returns the best string encoding for legacy format support.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontGetStringEncoding(_ font: CTFont) -> CFStringEncoding
```

## Parameters 

`font`  

The font reference.

## Return Value

The best string encoding for the font.

## See Also

### Working With Encoding

func CTFontCopyCharacterSet(CTFont) -> CFCharacterSet

Returns the Unicode character set of the font.

func CTFontCopySupportedLanguages(CTFont) -> CFArray

Returns an array of languages supported by the font.

