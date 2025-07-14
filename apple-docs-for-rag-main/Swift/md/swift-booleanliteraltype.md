

- Swift
-  BooleanLiteralType 

Type Alias

# BooleanLiteralType

The default type for an otherwise-unconstrained Boolean literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias BooleanLiteralType = Bool
```

## Discussion

When you create a constant or variable using one of the Boolean literals `true` or `false`, the resulting type is determined by the `BooleanLiteralType` alias. For example:

```
let isBool = true
print("isBool is a '\(type(of: isBool))'")
// Prints "isBool is a 'Bool'"
```

The type aliased by `BooleanLiteralType` must conform to the `ExpressibleByBooleanLiteral` protocol.

## See Also

### Basic Values

typealias IntegerLiteralType

The default type for an otherwise-unconstrained integer literal.

typealias FloatLiteralType

The default type for an otherwise-unconstrained floating-point literal.

