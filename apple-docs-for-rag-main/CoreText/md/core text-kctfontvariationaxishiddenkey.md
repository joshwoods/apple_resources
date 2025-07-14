

- Core Text
-  kCTFontVariationAxisHiddenKey 

Global Variable

# kCTFontVariationAxisHiddenKey

The key to find out if the axis is hidden.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCTFontVariationAxisHiddenKey: CFString
```

## Discussion

This key contains a doc://com.apple.documentation/documentation/corefoundation/cfboolean-s0p value that is kCFBooleanTrue when the font designer recommends the axis not be exposed directly to end users in application interfaces.

Reasons for setting this flag might include that the axis is intended only for programmatic interaction, or is intended for font-internal use by the font developer.

## See Also

### Constants

let kCTFontVariationAxisIdentifierKey: CFString

Key to get the variation axis identifier.

let kCTFontVariationAxisMinimumValueKey: CFString

Key to get the variation axis minimum value.

let kCTFontVariationAxisMaximumValueKey: CFString

Key to get the variation axis maximum value.

let kCTFontVariationAxisDefaultValueKey: CFString

Key to get the variation axis default value.

let kCTFontVariationAxisNameKey: CFString

Key to get the localized variation axis name string.

