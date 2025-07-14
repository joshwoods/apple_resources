

- Swift
- UInt128
-  init(truncatingIfNeeded:) 

Initializer

# init(truncatingIfNeeded:)

Creates a new instance from the bit pattern of the given instance by sign-extending or truncating to fit this type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(truncatingIfNeeded source: T) where T : BinaryInteger
```

## Parameters 

`source`  

An integer to convert to this type.

## Discussion

When the bit width of `T` (the type of `source`) is equal to or greater than this type’s bit width, the result is the truncated least-significant bits of `source`. For example, when converting a 16-bit value to an 8-bit type, only the lower 8 bits of `source` are used.

```
let p: Int16 = -500
// 'p' has a binary representation of 11111110_00001100
let q = Int8(truncatingIfNeeded: p)
// q == 12
// 'q' has a binary representation of 00001100
```

When the bit width of `T` is less than this type’s bit width, the result is *sign-extended* to fill the remaining bits. That is, if `source` is negative, the result is padded with ones; otherwise, the result is padded with zeros.

```
let u: Int8 = 21
// 'u' has a binary representation of 00010101
let v = Int16(truncatingIfNeeded: u)
// v == 21
// 'v' has a binary representation of 00000000_00010101

let w: Int8 = -21
// 'w' has a binary representation of 11101011
let x = Int16(truncatingIfNeeded: w)
// x == -21
// 'x' has a binary representation of 11111111_11101011
let y = UInt16(truncatingIfNeeded: w)
// y == 65515
// 'y' has a binary representation of 11111111_11101011
```

