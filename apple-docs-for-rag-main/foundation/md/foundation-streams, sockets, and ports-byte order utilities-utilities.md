

- Foundation
- Streams, Sockets, and Ports
-  Byte Order Utilities 

API Collection

# Byte Order Utilities

Examine and manage the byte order of numbers communicated through network channels.

## Topics

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

func NSSwapHostFloatToBig(Float) -> NSSwappedFloat

Swaps the bytes of a number.

func NSSwapHostFloatToLittle(Float) -> NSSwappedFloat

Swaps the bytes of a number.

func NSSwapHostIntToBig(UInt32) -> UInt32

Swaps the bytes of a number.

func NSSwapHostIntToLittle(UInt32) -> UInt32

Swaps the bytes of a number.

func NSSwapHostLongLongToBig(UInt64) -> UInt64

Swaps the bytes of a number.

func NSSwapHostLongLongToLittle(UInt64) -> UInt64

Swaps the bytes of a number.

func NSSwapHostLongToBig(UInt) -> UInt

Swaps the bytes of a number.

func NSSwapHostLongToLittle(UInt) -> UInt

Swaps the bytes of a number.

func NSSwapHostShortToBig(UInt16) -> UInt16

Swaps the bytes of a number.

func NSSwapHostShortToLittle(UInt16) -> UInt16

Swaps the bytes of a number.

func NSSwapInt(UInt32) -> UInt32

Swaps the bytes of a number.

func NSSwapLittleDoubleToHost(NSSwappedDouble) -> Double

Swaps the bytes of a number.

func NSSwapLittleFloatToHost(NSSwappedFloat) -> Float

Swaps the bytes of a number.

func NSSwapLittleIntToHost(UInt32) -> UInt32

Swaps the bytes of a number.

func NSSwapLittleLongLongToHost(UInt64) -> UInt64

Swaps the bytes of a number.

func NSSwapLittleLongToHost(UInt) -> UInt

Swaps the bytes of a number.

func NSSwapLittleShortToHost(UInt16) -> UInt16

Swaps the bytes of a number.

func NSSwapLong(UInt) -> UInt

Swaps the bytes of a number.

func NSSwapLongLong(UInt64) -> UInt64

Swaps the bytes of a number.

func NSSwapShort(UInt16) -> UInt16

Swaps the bytes of a number.

### Constants

struct NSSwappedDouble

Opaque structure containing endian-independent `double` value.

struct NSSwappedFloat

Opaque type containing an endian-independent `float` value.

Byte Order

Recognize constants that specify a byte-order format.

