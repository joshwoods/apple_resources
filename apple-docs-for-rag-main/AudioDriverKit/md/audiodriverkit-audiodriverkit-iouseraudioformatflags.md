

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioFormatFlags 

Enumeration

# IOUserAudioFormatFlags

Flag values that provide more information about the format used by an audio stream basic description.

DriverKit 21.0+

``` source
enum IOUserAudioFormatFlags : uint32_t;
```

## Topics

### Numeric Representation Flags

FormatFlagIsFloat

A flag to indicate whether samples are floating-point values.

LinearPCMFormatFlagIsFloat

A flag to indicate whether PCM samples are floating-point values.

FormatFlagIsSignedInteger

A flag to indicate whether samples are signed or unsigned integers.

LinearPCMFormatFlagIsSignedInteger

A flag to indicate whether PCM samples are signed or unsigned integers.

### Bitwise Layout Flags

FormatFlagIsAlignedHigh

A flag to indicate whether sample bits use the high bits of the channel.

LinearPCMFormatFlagIsAlignedHigh

A flag to indicate whether PCM sample bits use the high bits of the channel.

FormatFlagIsPacked

A flag to indicate whether sample bits use all available bits of the channel.

LinearPCMFormatFlagIsPacked

A flag to indicate whether PCM sample bits use all available bits of the channel.

FormatFlagsNativeFloatPacked

A flag indicating native-endian packed floating-point values.

### Endianness Flags

FormatFlagIsBigEndian

A flag to indicate whether samples use big-endian values.

LinearPCMFormatFlagIsBigEndian

A flag to indicate whether PCM samples use big-endian values.

FormatFlagsNativeEndian

A flag to indicate whether samples use the platform’s native endianness for its values.

### Apple Lossless Flags

AppleLosslessFormatFlag_16BitSourceData

A flag to indicate Apple Lossless data that originated from 16-bit native endian-signed integer data.

AppleLosslessFormatFlag_20BitSourceData

A flag to indicate Apple Lossless data that originated from 20-bit native endian-signed integer data.

AppleLosslessFormatFlag_24BitSourceData

A flag to indicate Apple Lossless data that originated from 24-bit native endian-signed integer data.

AppleLosslessFormatFlag_32BitSourceData

A flag to indicate Apple Lossless data that originated from 32-bit native endian-signed integer data.

### Channel Layout Flags

FormatFlagIsNonInterleaved

A flag to indicate whether the channels interleave their samples in the data.

LinearPCMFormatFlagIsNonInterleaved

A flag to indicate whether PCM channels interleave their samples in the data.

### Mixability Flags

FormatFlagIsNonMixable

A flag to indicate whether the format can’t mix.

LinearPCMFormatFlagIsNonMixable

A flag to indicate whether the PCM format can’t mix.

### Sample Fraction Flags

LinearPCMFormatFlagsSampleFractionMask

A constant that indicates the bit position of a bit field within the flags, for use with fixed-point values.

LinearPCMFormatFlagsSampleFractionShift

A mask used to calculate the number of fractional bits in the flags field.

### Special Purpose Flags

FormatFlagsAreAllClear

A value indicating that all format flags are clear.

LinearPCMFormatFlagsAreAllClear

A value indicating that all PCM format flags are clear.

## See Also

### Identifying the Format

mFormatID

The audio format identifier indicating the general kind of data in the stream.

IOUserAudioFormatID

An enumeration of four character codes used to identify distinct audio data formats.

mFormatFlags

Audio format flags for the stream’s format.

