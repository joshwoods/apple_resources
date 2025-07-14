

- Core Foundation
-  Byte-Order Utilities 

API Collection

# Byte-Order Utilities

## Overview

When handling binary data transmitted or shared across platforms, you need be concerned with how each platform stores numerical values. A platform stores values either in big-endian or little-endian format. On big-endian machines, such as PowerPC machines, values are stored with the most-significant bytes first in memory; on little-endian machines, such as Pentium machines, values are stored with the least-significant bytes first. A multibyte value transmitted to a platform with a different format will be misinterpreted if it is not converted properly by one of the computers.

You identify the native format of the current platform using the CFByteOrderGetCurrent() function. Use functions such as CFSwapInt32BigToHost(_:) and CFConvertFloat32HostToSwapped(_:) to convert values between different byte order formats.

## Topics

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

func CFConvertFloat64HostToSwapped(Float64) -> CFSwappedFloat64

Converts a 64-bit float from the host’s native byte order to a platform-independent format.

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

func CFSwapInt32HostToBig(UInt32) -> UInt32

Converts a 32-bit integer from the host’s native byte order to big-endian format.

func CFSwapInt32HostToLittle(UInt32) -> UInt32

Converts a 32-bit integer from the host’s native byte order to little-endian format.

func CFSwapInt32LittleToHost(UInt32) -> UInt32

Converts a 32-bit integer from little-endian format to the host’s native byte order.

func CFSwapInt64(UInt64) -> UInt64

Swaps the bytes of a 64-bit integer.

func CFSwapInt64BigToHost(UInt64) -> UInt64

Converts a 64-bit integer from big-endian format to the host’s native byte order.

func CFSwapInt64HostToBig(UInt64) -> UInt64

Converts a 64-bit integer from the host’s native byte order to big-endian format.

func CFSwapInt64HostToLittle(UInt64) -> UInt64

Converts a 64-bit integer from the host’s native byte order to little-endian format.

func CFSwapInt64LittleToHost(UInt64) -> UInt64

Converts a 64-bit integer from little-endian format to the host’s native byte order.

### Data Types

struct CFSwappedFloat32

Structure holding a 32-bit float value in a platform-independentbyte order.

struct CFSwappedFloat64

Structure holding a 64-bit float value in a platform-independentbyte order.

### Constants

typealias CFByteOrder

Flags that identify byte order.

## See Also

### Related Documentation

Memory Management Programming Guide for Core Foundation

### Utilities

Base Utilities

Core Foundation URL Access Utilities

Preferences Utilities

Socket Name Server Utilities

Time Utilities

