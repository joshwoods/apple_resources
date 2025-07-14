

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isASCIIHexDigit 

Instance Property

# isASCIIHexDigit

A Boolean value indicating whether the scalar is an ASCII character commonly used for the representation of hexadecimal numbers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isASCIIHexDigit: Bool { get }
```

## Discussion

The only scalars for which this property is `true` are:

- U+0030…U+0039: DIGIT ZERO…DIGIT NINE

- U+0041…U+0046: LATIN CAPITAL LETTER A…LATIN CAPITAL LETTER F

- U+0061…U+0066: LATIN SMALL LETTER A…LATIN SMALL LETTER F

This property corresponds to the “ASCII_Hex_Digit” property in the Unicode Standard.

