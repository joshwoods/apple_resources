

- Swift
- Swift Standard Library
- Initialization with Literals
-  Default Literal Types 

API Collection

# Default Literal Types

Type aliases representing the concrete type that a literal takes when no other type information is provided.

## Overview

This example declares the `numberOfCookies` constant, using an integer literal to express its value:

```
let numberOfCookies = 5
// type(of: numberOfCookies) == Int.self
```

When a literal expression is written with no type information, Swift uses these type aliases to determine what type to use for the expression. In this case, the `numberOfCookies` constant has the default type for an integer literal, `Int`, as designated by the `IntegerLiteralType` type alias.

## Topics

### Basic Values

typealias BooleanLiteralType

The default type for an otherwise-unconstrained Boolean literal.

typealias IntegerLiteralType

The default type for an otherwise-unconstrained integer literal.

typealias FloatLiteralType

The default type for an otherwise-unconstrained floating-point literal.

### Strings and Text

typealias StringLiteralType

The default type for an otherwise-unconstrained string literal.

typealias ExtendedGraphemeClusterType

The default type for an otherwise-unconstrained Unicode extended grapheme cluster literal.

typealias UnicodeScalarType

The default type for an otherwise-unconstrained unicode scalar literal.

