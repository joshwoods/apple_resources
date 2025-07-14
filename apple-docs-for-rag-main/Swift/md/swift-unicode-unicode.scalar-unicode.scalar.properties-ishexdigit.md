

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isHexDigit 

Instance Property

# isHexDigit

A Boolean value indicating whether the scalar is one that is commonly used for the representation of hexadecimal numbers or a compatibility equivalent.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isHexDigit: Bool { get }
```

## Discussion

This property is `true` for all scalars for which `isASCIIHexDigit` is `true` as well as for their CJK halfwidth and fullwidth variants.

This property corresponds to the “Hex_Digit” property in the Unicode Standard.

