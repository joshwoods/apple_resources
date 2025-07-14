

- Swift
- Unicode
- Unicode.Scalar
-  init(unicodeScalarLiteral:) 

Initializer

# init(unicodeScalarLiteral:)

Creates a Unicode scalar with the specified value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(unicodeScalarLiteral value: Unicode.Scalar)
```

## Discussion

Do not call this initializer directly. It may be used by the compiler when you use a string literal to initialize a `Unicode.Scalar` instance.

```
let letterK: Unicode.Scalar = "K"
print(letterK)
// Prints "K"
```

In this example, the assignment to the `letterK` constant is handled by this initializer behind the scenes.

## See Also

### Creating a Scalar

init(UInt8)

Creates a Unicode scalar with the specified numeric value.

init(Unicode.Scalar)

Creates a duplicate of the given Unicode scalar.

init?(UInt32)

Creates a Unicode scalar with the specified numeric value.

init?(UInt16)

Creates a Unicode scalar with the specified numeric value.

init?(Int)

Creates a Unicode scalar with the specified numeric value.

init?(String)

Instantiates an instance of the conforming type from a string representation.

