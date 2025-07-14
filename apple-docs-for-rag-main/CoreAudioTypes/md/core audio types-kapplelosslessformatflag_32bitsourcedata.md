

- Core Audio Types
-  kAppleLosslessFormatFlag_32BitSourceData 

Global Variable

# kAppleLosslessFormatFlag_32BitSourceData

A flag that indicates Apple Lossless data sourced from 32-bit native endian signed integer data.

iOS 2.0+iPadOS 2.0+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var kAppleLosslessFormatFlag_32BitSourceData: AudioFormatFlags { get }
```

## See Also

### Format flags

var kAppleLosslessFormatFlag_16BitSourceData: AudioFormatFlags

A flag that indicates Apple Lossless data sourced from 16-bit native endian signed integer data.

var kAppleLosslessFormatFlag_20BitSourceData: AudioFormatFlags

A flag that indicates Apple Lossless data sourced from 20-bit native endian signed integer data aligned high in 24 bits.

var kAppleLosslessFormatFlag_24BitSourceData: AudioFormatFlags

A flag that indicates Apple Lossless data sourced from 24-bit native endian signed integer data.

var kAudioFormatFlagIsAlignedHigh: AudioFormatFlags

A flag that indicates whether placement of the sample bits is with the high or low bits of the channel.

var kAudioFormatFlagIsBigEndian: AudioFormatFlags

A flag that indicates whether the format is big or little endian.

var kAudioFormatFlagIsFloat: AudioFormatFlags

A flag that indicates whether the format is floating point or integer.

var kAudioFormatFlagIsNonInterleaved: AudioFormatFlags

A flag that indicates whether the samples for each channel or frame are continguously located, and whether the layout of the channels or frames is end-to-end.

var kAudioFormatFlagIsNonMixable: AudioFormatFlags

A flag that indicates the format is nonmixable.

var kAudioFormatFlagIsPacked: AudioFormatFlags

A flag that indicates whether placement of the sample bits occupy the entire available bits of the channel.

var kAudioFormatFlagIsSignedInteger: AudioFormatFlags

A flag that indicates whether the format is signed or unsigned integer.

var kAudioFormatFlagsAreAllClear: AudioFormatFlags

A flag that indicates whether all the flags are clear.

var kAudioFormatFlagsNativeEndian: AudioFormatFlags

A flag that specifies whether the format is big endian, depending on the endianness of the processor at build time.

var kAudioFormatFlagsNativeFloatPacked: AudioFormatFlags

The flags for the canonical format of fully packed, native endian floating-point data.

var kLinearPCMFormatFlagIsAlignedHigh: AudioFormatFlags

A flag that indicates whether placement of the sample bits is with the high or low bits of the channel.

var kLinearPCMFormatFlagIsBigEndian: AudioFormatFlags

A flag that indicates whether the format is big or little endian.

