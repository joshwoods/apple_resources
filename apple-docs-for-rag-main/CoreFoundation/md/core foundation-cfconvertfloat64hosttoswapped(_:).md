

- Core Foundation
-  CFConvertFloat64HostToSwapped(\_:) 

Function

# CFConvertFloat64HostToSwapped(\_:)

Converts a 64-bit float from the host’s native byte order to a platform-independent format.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFConvertFloat64HostToSwapped(_ arg: Float64) -> CFSwappedFloat64
```

## Parameters 

`arg`  

The real value to convert.

## Return Value

A structure holding the real value in a canonical byte order.

## See Also

### Core Foundation Byte Order Utilities Miscellaneous Functions

func CFByteOrderGetCurrent() -> CFByteOrder

Returns the byte order of the current computer.

func CFConvertDoubleHostToSwapped(Double) -> CFSwappedFloat64

Converts a 64-bit double from the host’s native byte order to a platform-independent format.

func CFConvertDoubleSwappedToHost(CFSwappedFloat64) -> Double

Converts a 64-bit double from a platform-independent format to the host’s native byte order.

func CFConvertFloat32HostToSwapped(Float32) -> CFSwappedFloat32

Converts a 32-bit float from the host’s native byte order to a platform-independent format.

func CFConvertFloat32SwappedToHost(CFSwappedFloat32) -> Float32

Converts a 32-bit float from a platform-independent format to the host’s native byte order.

func CFConvertFloat64SwappedToHost(CFSwappedFloat64) -> Float64

Converts a 64-bit float from a platform-independent format to the host’s native byte order.

func CFConvertFloatHostToSwapped(Float) -> CFSwappedFloat32

Converts a 32-bit float from the host’s native byte order to a platform-independent format.

func CFConvertFloatSwappedToHost(CFSwappedFloat32) -> Float

Converts a 32-bit float from a platform-independent format to the host’s native byte order.

func CFSwapInt16(UInt16) -> UInt16

Swaps the bytes of a 16-bit integer.

func CFSwapInt16BigToHost(UInt16) -> UInt16

Converts a 16-bit integer from big-endian format to the host’s native byte order.

func CFSwapInt16HostToBig(UInt16) -> UInt16

Converts a 16-bit integer from the host’s native byte order to big-endian format.

func CFSwapInt16HostToLittle(UInt16) -> UInt16

Converts a 16-bit integer from the host’s native byte order to little-endian format.

func CFSwapInt16LittleToHost(UInt16) -> UInt16

Converts a 16-bit integer from little-endian format to the host’s native byte order.

func CFSwapInt32(UInt32) -> UInt32

Swaps the bytes of a 32-bit integer.

func CFSwapInt32BigToHost(UInt32) -> UInt32

Converts a 32-bit integer from big-endian format to the host’s native byte order.

