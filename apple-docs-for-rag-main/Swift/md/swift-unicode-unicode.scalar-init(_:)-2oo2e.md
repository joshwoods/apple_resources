

- Swift
- Unicode
- Unicode.Scalar
-  init(\_:) 

Initializer

# init(\_:)

Creates a Unicode scalar with the specified numeric value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ v: UInt8)
```

## Parameters 

`v`  

The code point to use for the scalar.

## Discussion

For example, the following code sample creates a `Unicode.Scalar` instance with a value of `"7"`:

```
let codepoint: UInt8 = 55
let seven = Unicode.Scalar(codepoint)
print(seven)
// Prints "7"
```

## See Also

### Creating a Scalar

init(Unicode.Scalar)

Creates a duplicate of the given Unicode scalar.

init?(UInt32)

Creates a Unicode scalar with the specified numeric value.

init?(UInt16)

Creates a Unicode scalar with the specified numeric value.

init?(Int)

Creates a Unicode scalar with the specified numeric value.

init(unicodeScalarLiteral: Unicode.Scalar)

Creates a Unicode scalar with the specified value.

init?(String)

Instantiates an instance of the conforming type from a string representation.

