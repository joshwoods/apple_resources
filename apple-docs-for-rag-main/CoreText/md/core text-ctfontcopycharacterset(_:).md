

- Core Text
-  CTFontCopyCharacterSet(\_:) 

Function

# CTFontCopyCharacterSet(\_:)

Returns the Unicode character set of the font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyCharacterSet(_ font: CTFont) -> CFCharacterSet
```

## Parameters 

`font`  

The font reference.

## Return Value

A retained reference to the font’s character set.

## Discussion

The returned character set covers the nominal referenced by the font’s Unicode `'cmap’` table.

## See Also

### Working With Encoding

func CTFontGetStringEncoding(CTFont) -> CFStringEncoding

Returns the best string encoding for legacy format support.

func CTFontCopySupportedLanguages(CTFont) -> CFArray

Returns an array of languages supported by the font.

