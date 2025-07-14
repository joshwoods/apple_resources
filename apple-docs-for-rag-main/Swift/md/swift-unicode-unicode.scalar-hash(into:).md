

- Swift
- Unicode
- Unicode.Scalar
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of this value by feeding them into the given hasher.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func hash(into hasher: inout Hasher)
```

## Parameters 

`hasher`  

The hasher to use when combining the components of this instance.

## See Also

### Inspecting a Scalar

var value: UInt32

A numeric representation of the Unicode scalar.

var properties: Unicode.Scalar.Properties

Properties of this scalar defined by the Unicode standard.

struct Properties

A value that provides access to properties of a Unicode scalar that are defined by the Unicode standard.

var isASCII: Bool

A Boolean value indicating whether the Unicode scalar is an ASCII character.

