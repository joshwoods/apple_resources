

- Swift
- UInt128
-  init(clamping:) 

Initializer

# init(clamping:)

Creates a new instance with the representable value that’s closest to the given integer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(clamping source: T) where T : BinaryInteger
```

## Parameters 

`source`  

An integer to convert to this type.

## Discussion

If the value passed as `source` is greater than the maximum representable value in this type, the result is the type’s `max` value. If `source` is less than the smallest representable value in this type, the result is the type’s `min` value.

In this example, `x` is initialized as an `Int8` instance by clamping `500` to the range `-128...127`, and `y` is initialized as a `UInt` instance by clamping `-500` to the range `0...UInt.max`.

```
let x = Int8(clamping: 500)
// x == 127
// x == Int8.max

let y = UInt(clamping: -500)
// y == 0
```

