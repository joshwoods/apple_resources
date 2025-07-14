

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  uppercaseMapping 

Instance Property

# uppercaseMapping

The uppercase mapping of the scalar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var uppercaseMapping: String { get }
```

## Discussion

This property is a `String`, not a `Unicode.Scalar` or `Character`, because some mappings may transform a scalar into multiple scalars or graphemes. For example, the German letter “ß” (U+00DF LATIN SMALL LETTER SHARP S) becomes “SS” (U+0053 LATIN CAPITAL LETTER S, U+0053 LATIN CAPITAL LETTER S) when converted to uppercase.

This property corresponds to the “Uppercase_Mapping” property in the Unicode Standard.

