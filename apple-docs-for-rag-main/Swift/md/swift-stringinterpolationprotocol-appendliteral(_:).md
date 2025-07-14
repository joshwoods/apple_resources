

- Swift
- StringInterpolationProtocol
-  appendLiteral(\_:) 

Instance Method

# appendLiteral(\_:)

Appends a literal segment to the interpolation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func appendLiteral(_ literal: Self.StringLiteralType)
```

**Required**

## Parameters 

`literal`  

A string literal containing the characters that appear next in the string literal.

## Discussion

Don’t call this method directly. Instead, initialize a variable or constant using a string literal with interpolated expressions.

Interpolated expressions don’t pass through this method; instead, Swift selects an overload of `appendInterpolation`. For more information, see the top-level `StringInterpolationProtocol` documentation.

