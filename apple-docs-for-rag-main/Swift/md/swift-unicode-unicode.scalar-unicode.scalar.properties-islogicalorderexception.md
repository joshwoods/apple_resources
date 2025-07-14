

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isLogicalOrderException 

Instance Property

# isLogicalOrderException

A Boolean value indicating whether the scalar requires special handling for operations involving ordering, such as sorting and searching.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isLogicalOrderException: Bool { get }
```

## Discussion

This property applies to a small number of spacing vowel letters occurring in some Southeast Asian scripts like Thai and Lao, which use a visual order display model. Such letters are stored in text ahead of syllable-initial consonants.

This property corresponds to the “Logical_Order_Exception” property in the Unicode Standard.

