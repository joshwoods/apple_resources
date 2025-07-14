

- Swift
- String
-  init(stringInterpolation:) 

Initializer

# init(stringInterpolation:)

Creates a new instance from an interpolated string literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(stringInterpolation: DefaultStringInterpolation)
```

Available when `StringInterpolation` is `DefaultStringInterpolation`.

## Discussion

Don’t call this initializer directly. It’s used by the compiler when you create a string using string interpolation. Instead, use string interpolation to create a new string by including values, literals, variables, or expressions enclosed in parentheses, prefixed by a backslash (`\(`…`)`).

```
let price = 2
let number = 3
let message = """
              If one cookie costs \(price) dollars, \
              \(number) cookies cost \(price * number) dollars.
              """
// message == "If one cookie costs 2 dollars, 3 cookies cost 6 dollars."
```

