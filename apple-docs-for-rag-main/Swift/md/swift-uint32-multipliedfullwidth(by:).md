

- Swift
- UInt32
-  multipliedFullWidth(by:) 

Instance Method

# multipliedFullWidth(by:)

Returns a tuple containing the high and low parts of the result of multiplying this value by the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func multipliedFullWidth(by other: UInt32) -> (high: UInt32, low: UInt32.Magnitude)
```

## Parameters 

`other`  

The value to multiply this value by.

## Return Value

A tuple containing the high and low parts of the result of multiplying this value and `other`.

## Discussion

Use this method to calculate the full result of a product that would otherwise overflow. Unlike traditional truncating multiplication, the `multipliedFullWidth(by:)` method returns a tuple containing both the `high` and `low` parts of the product of this value and `other`. The following example uses this method to multiply two `Int8` values that normally overflow when multiplied:

```
let x: Int8 = 48
let y: Int8 = -40
let result = x.multipliedFullWidth(by: y)
// result.high == -8
// result.low  == 128
```

The product of `x` and `y` is `-1920`, which is too large to represent in an `Int8` instance. The `high` and `low` components of the `result` value represent `-1920` when concatenated to form a double-width integer; that is, using `result.high` as the high byte and `result.low` as the low byte of an `Int16` instance.

```
let z = Int16(result.high) 

