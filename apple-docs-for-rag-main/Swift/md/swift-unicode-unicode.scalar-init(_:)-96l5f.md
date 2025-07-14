

- Swift
- Unicode
- Unicode.Scalar
-  init(\_:) 

Initializer

# init(\_:)

Creates a Unicode scalar with the specified numeric value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(_ v: Int)
```

## Parameters 

`v`  

The Unicode code point to use for the scalar. `v` must be a valid Unicode scalar value, in the ranges `0...0xD7FF` or `0xE000...0x10FFFF`. In case of an invalid unicode scalar value, nil is returned.

## Discussion

For example, the following code sample creates a `Unicode.Scalar` instance with a value of an emoji character:

```
let codepoint = 127881
let emoji = Unicode.Scalar(codepoint)!
print(emoji)
// Prints "🎉"
```

In case of an invalid input value, nil is returned.

```
let codepoint: UInt32 = extValue // This might be an invalid value.
if let emoji = Unicode.Scalar(codepoint) {
  print(emoji)
} else {
  // Do something else
}
```

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

init(unicodeScalarLiteral: Unicode.Scalar)

Creates a Unicode scalar with the specified value.

init?(String)

Instantiates an instance of the conforming type from a string representation.

