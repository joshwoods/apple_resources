

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isFullCompositionExclusion 

Instance Property

# isFullCompositionExclusion

A Boolean value indicating whether the scalar is excluded from composition when performing Unicode normalization.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isFullCompositionExclusion: Bool { get }
```

## Discussion

This property corresponds to the “Full_Composition_Exclusion” property in the Unicode Standard.

