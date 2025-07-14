

- AudioDriverKit
- AudioDriverKit
- IOUserAudioFormatFlags
-  FormatFlagIsAlignedHigh 

Enumeration Case

# FormatFlagIsAlignedHigh

A flag to indicate whether sample bits use the high bits of the channel.

DriverKit 21.0+

``` source
FormatFlagIsAlignedHigh
```

## Discussion

Set this value if sample bits use the high end of the channel; clear it to use the low end. This flag is only valid if FormatFlagIsPacked is clear.

## See Also

### Bitwise Layout Flags

LinearPCMFormatFlagIsAlignedHigh

A flag to indicate whether PCM sample bits use the high bits of the channel.

FormatFlagIsPacked

A flag to indicate whether sample bits use all available bits of the channel.

LinearPCMFormatFlagIsPacked

A flag to indicate whether PCM sample bits use all available bits of the channel.

FormatFlagsNativeFloatPacked

A flag indicating native-endian packed floating-point values.

