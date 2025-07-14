

- Core Text
-  CTFontCopyFeatures(\_:) 

Function

# CTFontCopyFeatures(\_:)

Returns an array of font features.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyFeatures(_ font: CTFont) -> CFArray?
```

## Parameters 

`font`  

The font reference.

## Return Value

An array of font feature dictionaries for the font reference.

## See Also

### Getting Font Features

func CTFontCopyFeatureSettings(CTFont) -> CFArray?

Returns an array of font feature-setting tuples.

