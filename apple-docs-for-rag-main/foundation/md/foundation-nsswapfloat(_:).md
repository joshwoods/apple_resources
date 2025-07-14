

- Foundation
-  NSSwapFloat(\_:) 

Function

# NSSwapFloat(\_:)

Swaps the bytes of a number.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSSwapFloat(_ x: NSSwappedFloat) -> NSSwappedFloat
```

## Discussion

Swaps the bytes of `x` and returns the resulting value. Bytes are swapped from each low-order position to the corresponding high-order position and vice versa. For example, if the bytes of `x` are numbered from 1 to 4, this function swaps bytes 1 and 4, and bytes 2 and 3.

## See Also

### Related Documentation

func NSSwapLong(UInt) -> UInt

Swaps the bytes of a number.

func NSSwapDouble(NSSwappedDouble) -> NSSwappedDouble

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

func NSSwapHostDoubleToBig(Double) -> NSSwappedDouble

Swaps the bytes of a number.

func NSSwapHostDoubleToLittle(Double) -> NSSwappedDouble

Swaps the bytes of a number.

func NSSwapHostFloatToBig(Float) -> NSSwappedFloat

Swaps the bytes of a number.

