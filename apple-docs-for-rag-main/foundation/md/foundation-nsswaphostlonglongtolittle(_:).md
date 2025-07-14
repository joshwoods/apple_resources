

- Foundation
-  NSSwapHostLongLongToLittle(\_:) 

Function

# NSSwapHostLongLongToLittle(\_:)

Swaps the bytes of a number.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSSwapHostLongLongToLittle(_ x: UInt64) -> UInt64
```

## Discussion

Converts the value in `x`, specified in the current endian format, to little-endian format and returns the resulting value. If it is necessary to swap the bytes, this function calls NSSwapLongLong(_:) to perform the swap.

## See Also

### Related Documentation

func NSSwapLittleLongLongToHost(UInt64) -> UInt64

Swaps the bytes of a number.

func NSSwapHostLongLongToBig(UInt64) -> UInt64

Swaps the bytes of a number.

### Functions

func NSConvertHostDoubleToSwapped(Double) -> NSSwappedDouble

Performs a type conversion.

func NSConvertHostFloatToSwapped(Float) -> NSSwappedFloat

Performs a type conversion.

func NSConvertSwappedDoubleToHost(NSSwappedDouble) -> Double

Performs a type conversion.

func NSConvertSwappedFloatToHost(NSSwappedFloat) -> Float

Performs a type conversion.

func NSHostByteOrder() -> Int

Returns the endian format.

func NSSwapBigDoubleToHost(NSSwappedDouble) -> Double

Swaps the bytes of a number.

func NSSwapBigFloatToHost(NSSwappedFloat) -> Float

Swaps the bytes of a number.

func NSSwapBigIntToHost(UInt32) -> UInt32

Swaps the bytes of a number.

func NSSwapBigLongLongToHost(UInt64) -> UInt64

Swaps the bytes of a number.

func NSSwapBigLongToHost(UInt) -> UInt

Swaps the bytes of a number.

func NSSwapBigShortToHost(UInt16) -> UInt16

Swaps the bytes of a number.

func NSSwapDouble(NSSwappedDouble) -> NSSwappedDouble

Swaps the bytes of a number.

func NSSwapFloat(NSSwappedFloat) -> NSSwappedFloat

Swaps the bytes of a number.

func NSSwapHostDoubleToBig(Double) -> NSSwappedDouble

Swaps the bytes of a number.

func NSSwapHostDoubleToLittle(Double) -> NSSwappedDouble

Swaps the bytes of a number.

