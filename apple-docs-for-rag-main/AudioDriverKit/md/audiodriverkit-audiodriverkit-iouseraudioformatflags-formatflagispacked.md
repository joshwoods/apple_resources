

- AudioDriverKit
- AudioDriverKit
- IOUserAudioFormatFlags
-  FormatFlagIsPacked 

Enumeration Case

# FormatFlagIsPacked

A flag to indicate whether sample bits use all available bits of the channel.

DriverKit 21.0+

``` source
FormatFlagIsPacked
```

## Discussion

Set this value to use all bits with in the channel; clear to use either the high or low end, as indicated by FormatFlagIsAlignedHigh. Even if this flag is clear, the framework assumes it’s actually set if the IOUserAudioStreamBasicDescription contains the relationship `((mBitsPerSample / 8) * mChannelsPerFrame) == mBytesPerFrame`.

## See Also

### Bitwise Layout Flags

FormatFlagIsAlignedHigh

A flag to indicate whether sample bits use the high bits of the channel.

LinearPCMFormatFlagIsAlignedHigh

A flag to indicate whether PCM sample bits use the high bits of the channel.

LinearPCMFormatFlagIsPacked

A flag to indicate whether PCM sample bits use all available bits of the channel.

FormatFlagsNativeFloatPacked

A flag indicating native-endian packed floating-point values.

