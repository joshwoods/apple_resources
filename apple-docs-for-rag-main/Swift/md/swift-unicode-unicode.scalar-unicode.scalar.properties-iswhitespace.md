

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isWhitespace 

Instance Property

# isWhitespace

A Boolean value indicating whether the scalar is a whitespace character.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isWhitespace: Bool { get }
```

## Discussion

This property is `true` for scalars that are spaces, separator characters, and other control characters that should be treated as whitespace for the purposes of parsing text elements.

This property corresponds to the “White_Space” property in the Unicode Standard.

