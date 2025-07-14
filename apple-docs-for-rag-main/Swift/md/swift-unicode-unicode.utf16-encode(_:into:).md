

- Swift
- Unicode
- Unicode.UTF16
-  encode(\_:into:) 

Type Method

# encode(\_:into:)

Encodes a Unicode scalar as a series of code units by calling the given closure on each code unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func encode(
    _ input: Unicode.Scalar,
    into processCodeUnit: (Unicode.UTF16.CodeUnit) -> Void
)
```

## Parameters 

`input`  

The Unicode scalar value to encode.

`processCodeUnit`  

A closure that processes one code unit argument at a time.

## Discussion

For example, the musical fermata symbol (“𝄐”) is a single Unicode scalar value (`\u{1D110}`) but requires two code units for its UTF-16 representation. The following code encodes a fermata in UTF-16:

```
var codeUnits: [UTF16.CodeUnit] = []
UTF16.encode("𝄐", into: { codeUnits.append($0) })
print(codeUnits)
// Prints "[55348, 56592]"
```

