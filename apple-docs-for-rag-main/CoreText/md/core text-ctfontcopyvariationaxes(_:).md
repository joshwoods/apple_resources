

- Core Text
-  CTFontCopyVariationAxes(\_:) 

Function

# CTFontCopyVariationAxes(\_:)

Returns an array of variation axes.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyVariationAxes(_ font: CTFont) -> CFArray?
```

## Parameters 

`font`  

The font reference.

## Return Value

An array of variation axes dictionaries. Each variation axis dictionary contains the five variation axis keys listed in Font Variation Axis Dictionary Keys.

## See Also

### Working With Font Variations

func CTFontCopyVariation(CTFont) -> CFDictionary?

Returns a variation dictionary from the font reference.

