

- Core Audio Types
-  Audio Format Flags 

API Collection

# Audio Format Flags

Commonly used combinations of data format flags for an audio stream description.

## Overview

Prefer using fixed-point formats in iOS and floating-point formats in macOS.

## Topics

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

var kLinearPCMFormatFlagIsBigEndian: AudioFormatFlags

A flag that indicates whether the format is big or little endian.

var kLinearPCMFormatFlagIsFloat: AudioFormatFlags

A flag that indicates whether the format is floating point or integer.

var kLinearPCMFormatFlagIsNonInterleaved: AudioFormatFlags

A flag that indicates whether the samples for each channel or frame are continguously located, and whether the layout of the channels or frames is end-to-end.

var kLinearPCMFormatFlagIsNonMixable: AudioFormatFlags

A flag that indicates the format is nonmixable.

var kLinearPCMFormatFlagIsPacked: AudioFormatFlags

A flag that indicates whether placement of the sample bits occupy the entire available bits of the channel.

var kLinearPCMFormatFlagIsSignedInteger: AudioFormatFlags

A flag that indicates whether the format is signed or unsigned integer.

var kLinearPCMFormatFlagsAreAllClear: AudioFormatFlags

A flag that indicates whether all the flags are clear.

var kLinearPCMFormatFlagsSampleFractionMask: AudioFormatFlags

A flag that indicates the sample fraction mask.

var kLinearPCMFormatFlagsSampleFractionShift: AudioFormatFlags

A flag that indicates the bit position of the PCM flag’s 6-bit bitfield.

var kAudioFormatFlagsAudioUnitCanonical: AudioFormatFlags

The flags for the canonical audio unit and processing sample type.

Deprecated

var kAudioFormatFlagsCanonical: AudioFormatFlags

The set of flags for the canonical input-output audio sample type.

Deprecated

## See Also

### Streams

struct AudioStreamBasicDescription

A format specification for an audio stream.

struct AudioStreamPacketDescription

A value that describes a packet in a buffer of audio data.

typealias AudioFormatFlags

A type definition for audio format flags.

typealias AudioFormatID

A type definition for audio format identifiers.

Audio Format Identifiers

Identifiers for supported audio formats.

let kAudioStreamAnyRate: Float64

A value that indicates that an audio stream can use any sample rate.

enum MPEG4ObjectID

Constants that define the type of MPEG-4 audio data.

Deprecated

