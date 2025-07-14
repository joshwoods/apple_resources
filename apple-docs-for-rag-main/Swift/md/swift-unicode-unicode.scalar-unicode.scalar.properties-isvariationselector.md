

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isVariationSelector 

Instance Property

# isVariationSelector

A Boolean value indicating whether the scalar is a variation selector.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isVariationSelector: Bool { get }
```

## Discussion

Variation selectors allow rendering engines that support them to choose different glyphs to display for a particular code point.

This property corresponds to the “Variation_Selector” property in the Unicode Standard.

