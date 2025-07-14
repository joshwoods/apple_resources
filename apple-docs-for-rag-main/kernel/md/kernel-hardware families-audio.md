

- Kernel
- Hardware Families
-  Audio 

API Collection

# Audio

Implement a driver that interacts with audio hardware.

## Topics

### Interfaces

IOAudioLevelControl

IOAudioSelectorControl

IOAudioToggleControl

IOAudioControl

Represents any controllable attribute of an IOAudioDevice.

IOAudioEngine

Abstract base class for a single audio audio / I/O engine.

IOAudioStream

This class wraps a single sample buffer in an audio driver.

IOAudioPort

Represents a logical or physical port or functional unit in an audio device.

### Devices

IOAudioDevice

Abstract base class for a single piece of audio hardware. The IOAudioDevice provides the central coordination point for an audio driver.

### User-Space Access

IOAudioControlUserClient

IOAudioEngineUserClient

### Descriptors

IOAudioBufferDataDescriptor

IOAudioSampleIntervalDescriptor

IOAudioStreamDataDescriptor

### Audio Data

IOAudioEngineNotifications

IOAudioEngineTraps

IOAudioSampleRate

IOAudioStreamFormat

IOAudioStreamFormatExtension

IOAudioTimeStamp

IOAudioClientBuffer

IOAudioClientBuffer64

IOAudioClientBufferExtendedInfo

IOAudioClientBufferExtendedInfo64

IOAudioEnginePosition

Represents a position in an audio audio engine.

IOAF_bcopy_WriteCombine

An efficient bcopy from "write combine" memory to regular memory. It is safe to assume that all memory has been copied when the function has completed

UInt64mult

### Conversions

IOAF_Float32ToInt8

IOAF_Float32ToNativeInt16

Converts 32-bit floating point to native 16-bit integer

IOAF_Float32ToNativeInt24

Converts 32-bit floating point to native 24-bit integer

IOAF_Float32ToNativeInt32

Converts 32-bit floating point to native 32-bit integer

IOAF_Float32ToSwapInt16

Converts 32-bit floating point to non-native 16-bit integer

IOAF_Float32ToSwapInt24

Converts 32-bit floating point to non-native 24-bit integer

IOAF_Float32ToSwapInt32

Converts 32-bit floating point to non-native 32-bit integer

IOAF_Int8ToFloat32

IOAF_NativeInt16ToFloat32

Converts native 16-bit integer float to 32-bit float

IOAF_NativeInt24ToFloat32

Converts native 24-bit integer float to 32-bit float

IOAF_NativeInt32ToFloat32

Converts native 32-bit integer float to 32-bit float

IOAF_SwapInt16ToFloat32

Converts non-native 16-bit integer float to 32-bit float

IOAF_SwapInt24ToFloat32

Converts non-native 24-bit integer float to 32-bit float

IOAF_SwapInt32ToFloat32

Converts non-native 32-bit integer float to 32-bit float

## See Also

### Interfaces

Graphics and Displays

Implement a driver that interacts with graphics and video hardware.

HID

Implement a driver that interacts with human interface devices, such as mice and keyboards.

Network

Implement a driver that interacts with network interfaces such as Ethernet adaptors.

SCSI

Implement a driver that supports Small Computer System Interface (SCSI) protocols.

Mass Storage

Implement a driver that communicates with CD, DVD, or other mass storage devices.

