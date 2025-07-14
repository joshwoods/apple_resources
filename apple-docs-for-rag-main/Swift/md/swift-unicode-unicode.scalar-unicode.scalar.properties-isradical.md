

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isRadical 

Instance Property

# isRadical

A Boolean value indicating whether the scalar is a radical component of CJK characters, Tangut characters, or Yi syllables.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isRadical: Bool { get }
```

## Discussion

These scalars are often the components of ideographic description sequences, as defined by the `isIDSBinaryOperator` and `isIDSTrinaryOperator` properties.

This property corresponds to the “Radical” property in the Unicode Standard.

