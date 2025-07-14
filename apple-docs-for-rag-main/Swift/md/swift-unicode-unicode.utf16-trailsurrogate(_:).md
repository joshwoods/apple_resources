

- Swift
- Unicode
- Unicode.UTF16
-  trailSurrogate(\_:) 

Type Method

# trailSurrogate(\_:)

Returns the low-surrogate code unit of the surrogate pair representing the specified Unicode scalar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func trailSurrogate(_ x: Unicode.Scalar) -> UTF16.CodeUnit
```

## Parameters 

`x`  

A Unicode scalar value. `x` must be represented by a surrogate pair when encoded in UTF-16. To check whether `x` is represented by a surrogate pair, use `UTF16.width(x) == 2`.

## Return Value

The trailing surrogate code unit of `x` when encoded in UTF-16.

## Discussion

Because a Unicode scalar value can require up to 21 bits to store its value, some Unicode scalars are represented in UTF-16 by a pair of 16-bit code units. The first and second code units of the pair, designated *leading* and *trailing* surrogates, make up a *surrogate pair*.

```
let apple: Unicode.Scalar = "🍎"
print(UTF16.trailSurrogate(apple))
// Prints "57166"
```

