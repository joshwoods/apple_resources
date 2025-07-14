

- Swift
- Unicode
- Unicode.Scalar
-  properties 

Instance Property

# properties

Properties of this scalar defined by the Unicode standard.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var properties: Unicode.Scalar.Properties { get }
```

## Discussion

Use this property to access the Unicode properties of a Unicode scalar value. The following code tests whether a string contains any math symbols:

```
let question = "Which is larger, 3 * 3 * 3 or 10 + 10 + 10?"
let hasMathSymbols = question.unicodeScalars.contains(where: {
    $0.properties.isMath
})
// hasMathSymbols == true
```

## See Also

### Inspecting a Scalar

var value: UInt32

A numeric representation of the Unicode scalar.

struct Properties

A value that provides access to properties of a Unicode scalar that are defined by the Unicode standard.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var isASCII: Bool

A Boolean value indicating whether the Unicode scalar is an ASCII character.

