

- Swift
- Unicode
- Unicode.UTF32
-  encode(\_:into:) 

Type Method

# encode(\_:into:)

Encodes a Unicode scalar as a UTF-32 code unit by calling the given closure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func encode(
    _ input: Unicode.Scalar,
    into processCodeUnit: (Unicode.UTF32.CodeUnit) -> Void
)
```

## Parameters 

`input`  

The Unicode scalar value to encode.

`processCodeUnit`  

A closure that processes one code unit argument at a time.

## Discussion

For example, like every Unicode scalar, the musical fermata symbol (“𝄐”) can be represented in UTF-32 as a single code unit. The following code encodes a fermata in UTF-32:

```
var codeUnit: UTF32.CodeUnit = 0
UTF32.encode("𝄐", into: { codeUnit = $0 })
print(codeUnit)
// Prints "119056"
```

