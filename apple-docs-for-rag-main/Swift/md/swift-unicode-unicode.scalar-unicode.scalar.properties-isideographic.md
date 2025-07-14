

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isIdeographic 

Instance Property

# isIdeographic

A Boolean value indicating whether the scalar is considered to be a CJKV (Chinese, Japanese, Korean, and Vietnamese) or other siniform (Chinese writing-related) ideograph.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isIdeographic: Bool { get }
```

## Discussion

This property roughly defines the class of “Chinese characters” and does not include characters of other logographic scripts such as Cuneiform or Egyptian Hieroglyphs.

This property corresponds to the “Ideographic” property in the Unicode Standard.

