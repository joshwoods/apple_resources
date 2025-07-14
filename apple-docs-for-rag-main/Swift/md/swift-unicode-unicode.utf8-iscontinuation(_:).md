

- Swift
- Unicode
- Unicode.UTF8
-  isContinuation(\_:) 

Type Method

# isContinuation(\_:)

Returns a Boolean value indicating whether the specified code unit is a UTF-8 continuation byte.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func isContinuation(_ byte: Unicode.UTF8.CodeUnit) -> Bool
```

## Parameters 

`byte`  

A UTF-8 code unit.

## Return Value

`true` if `byte` is a continuation byte; otherwise, `false`.

## Discussion

Continuation bytes take the form `0b10xxxxxx`. For example, a lowercase “e” with an acute accent above it (`"é"`) uses 2 bytes for its UTF-8 representation: `0b11000011` (195) and `0b10101001` (169). The second byte is a continuation byte.

```
let eAcute = "é"
for codeUnit in eAcute.utf8 {
    print(codeUnit, UTF8.isContinuation(codeUnit))
}
// Prints "195 false"
// Prints "169 true"
```

