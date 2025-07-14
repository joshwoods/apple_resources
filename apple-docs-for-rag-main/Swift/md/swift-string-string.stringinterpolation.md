

- Swift
- String
-  String.StringInterpolation 

Type Alias

# String.StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias StringInterpolation = DefaultStringInterpolation
```

## Discussion

The `StringLiteralType` of an interpolation type must match the `StringLiteralType` of the conforming type.

