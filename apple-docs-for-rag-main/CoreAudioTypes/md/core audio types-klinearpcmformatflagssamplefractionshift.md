

- Core Audio Types
-  kLinearPCMFormatFlagsSampleFractionShift 

Global Variable

# kLinearPCMFormatFlagsSampleFractionShift

A flag that indicates the bit position of the PCM flag’s 6-bit bitfield.

iOS 2.0+iPadOS 2.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var kLinearPCMFormatFlagsSampleFractionShift: AudioFormatFlags { get }
```

## Discussion

The linear PCM flags contain a 6-bit bitfield that indicates to interpret an integer format as fixed point. The value indicates the number of bits used to represent the fractional portion of each sample value. This constant indicates the bit position (counting from the right) of the bitfield in mFormatFlags.

## See Also

### Format flags

var kAppleLosslessFormatFlag_16BitSourceData: AudioFormatFlags

A flag that indicates Apple Lossless data sourced from 16-bit native endian signed integer data.

var kAppleLosslessFormatFlag_20BitSourceData: AudioFormatFlags

A flag that indicates Apple Lossless data sourced from 20-bit native endian signed integer data aligned high in 24 bits.

var kAppleLosslessFormatFlag_24BitSourceData: AudioFormatFlags

A flag that indicates Apple Lossless data sourced from 24-bit native endian signed integer data.

var kAppleLosslessFormatFlag_32BitSourceData: AudioFormatFlags

A flag that indicates Apple Lossless data sourced from 32-bit native endian signed integer data.

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

