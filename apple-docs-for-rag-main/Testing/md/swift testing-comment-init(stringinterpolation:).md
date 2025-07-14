

- Swift Testing
- Comment
-  init(stringInterpolation:) 

Initializer

# init(stringInterpolation:)

Creates a new instance from an interpolated string literal.

Swift TestingSwiftiOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

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

