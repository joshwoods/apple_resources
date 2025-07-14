

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isMath 

Instance Property

# isMath

A Boolean value indicating whether the scalar is one that naturally appears in mathematical contexts.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isMath: Bool { get }
```

## Discussion

The set of scalars for which this property is `true` includes mathematical operators and symbols as well as specific Greek and Hebrew letter variants that are categorized as symbols. Notably, it does *not* contain the standard digits or Latin/Greek letter blocks; instead, it contains the mathematical Latin, Greek, and Arabic letters and numbers defined in the Supplemental Multilingual Plane.

This property corresponds to the “Math” and the “Other_Math” properties in the Unicode Standard.

