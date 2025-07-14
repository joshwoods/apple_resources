

- Swift
- BinaryInteger
-  init(clamping:) 

Initializer

# init(clamping:)

Creates a new instance with the representable value that’s closest to the given integer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(clamping source: T) where T : BinaryInteger
```

**Required** Default implementation provided.

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

## Default Implementations

### BinaryInteger Implementations

init&lt;Other>(clamping: Other)

Creates a new instance with the representable value that’s closest to the given integer.

## See Also

### Converting Integers

init&lt;T>(T)

Creates a new instance from the given integer.

**Required** Default implementations provided.

init&lt;T>(truncatingIfNeeded: T)

Creates a new instance from the bit pattern of the given instance by sign-extending or truncating to fit this type.

**Required** Default implementation provided.

