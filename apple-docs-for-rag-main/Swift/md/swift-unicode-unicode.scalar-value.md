

- Swift
- Unicode
- Unicode.Scalar
-  value 

Instance Property

# value

A numeric representation of the Unicode scalar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var value: UInt32 { get }
```

## See Also

### Inspecting a Scalar

var properties: Unicode.Scalar.Properties

Properties of this scalar defined by the Unicode standard.

struct Properties

A value that provides access to properties of a Unicode scalar that are defined by the Unicode standard.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var isASCII: Bool

A Boolean value indicating whether the Unicode scalar is an ASCII character.

