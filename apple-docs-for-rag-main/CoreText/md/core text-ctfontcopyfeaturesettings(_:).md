

- Core Text
-  CTFontCopyFeatureSettings(\_:) 

Function

# CTFontCopyFeatureSettings(\_:)

Returns an array of font feature-setting tuples.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyFeatureSettings(_ font: CTFont) -> CFArray?
```

## Parameters 

`font`  

The font reference.

## Return Value

A normalized array of font feature-setting dictionaries. The array contains only the non-default settings that should be applied to the font, or `NULL` if the default settings should be used.

## Discussion

A feature-setting dictionary is a tuple of a kCTFontFeatureTypeIdentifierKey key-value pair and a kCTFontFeatureSelectorIdentifierKey key-value pair. Each setting dictionary indicates which setting is enabled. It is the caller’s responsibility to handle exclusive and nonexclusive settings as necessary.

The feature settings are verified against those that the font supports and any that do not apply are removed. Further, feature settings that represent a default setting for the font are also removed.

## See Also

### Getting Font Features

func CTFontCopyFeatures(CTFont) -> CFArray?

Returns an array of font features.

