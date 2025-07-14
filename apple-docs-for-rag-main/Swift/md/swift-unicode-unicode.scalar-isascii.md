

- Swift
- Unicode
- Unicode.Scalar
-  isASCII 

Instance Property

# isASCII

A Boolean value indicating whether the Unicode scalar is an ASCII character.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isASCII: Bool { get }
```

## Discussion

ASCII characters have a scalar value between 0 and 127, inclusive. For example:

```
let canyon = "Cañón"
for scalar in canyon.unicodeScalars {
    print(scalar, scalar.isASCII, scalar.value)
}
// Prints "C true 67"
// Prints "a true 97"
// Prints "ñ false 241"
// Prints "ó false 243"
// Prints "n true 110"
```

## See Also

### Inspecting a Scalar

var value: UInt32

A numeric representation of the Unicode scalar.

var properties: Unicode.Scalar.Properties

Properties of this scalar defined by the Unicode standard.

struct Properties

A value that provides access to properties of a Unicode scalar that are defined by the Unicode standard.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

