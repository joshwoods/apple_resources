

- Core Text
-  CTFontCopyVariation(\_:) 

Function

# CTFontCopyVariation(\_:)

Returns a variation dictionary from the font reference.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyVariation(_ font: CTFont) -> CFDictionary?
```

## Parameters 

`font`  

The font reference.

## Return Value

The current variation instance as a dictionary.

## Discussion

The keys for each variation correspond to the variation identifier obtained via kCTFontVariationAxisIdentifierKey, which represents the four-character axis code as a CFNumber object.

## See Also

### Working With Font Variations

func CTFontCopyVariationAxes(CTFont) -> CFArray?

Returns an array of variation axes.

