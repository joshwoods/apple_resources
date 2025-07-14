

- Foundation
-  NSConvertHostDoubleToSwapped(\_:) 

Function

# NSConvertHostDoubleToSwapped(\_:)

Performs a type conversion.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSConvertHostDoubleToSwapped(_ x: Double) -> NSSwappedDouble
```

## Discussion

Converts the double value in `x` to a value whose bytes can be swapped. This function does not actually swap the bytes of `x`. You should not need to call this function directly.

## See Also

### Related Documentation

func NSSwapHostDoubleToLittle(Double) -> NSSwappedDouble

Swaps the bytes of a number.

func NSSwapHostDoubleToBig(Double) -> NSSwappedDouble

Swaps the bytes of a number.

### Functions

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

func NSSwapHostFloatToBig(Float) -> NSSwappedFloat

Swaps the bytes of a number.

