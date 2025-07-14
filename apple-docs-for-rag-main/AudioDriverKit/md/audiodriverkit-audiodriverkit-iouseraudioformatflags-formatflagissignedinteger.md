

- AudioDriverKit
- AudioDriverKit
- IOUserAudioFormatFlags
-  FormatFlagIsSignedInteger 

Enumeration Case

# FormatFlagIsSignedInteger

A flag to indicate whether samples are signed or unsigned integers.

DriverKit 21.0+

``` source
FormatFlagIsSignedInteger
```

## Discussion

Set this value for signed integers; clear it for unsigned. This flag is only valid if FormatFlagIsFloat is clear.

## See Also

### Numeric Representation Flags

FormatFlagIsFloat

A flag to indicate whether samples are floating-point values.

LinearPCMFormatFlagIsFloat

A flag to indicate whether PCM samples are floating-point values.

LinearPCMFormatFlagIsSignedInteger

A flag to indicate whether PCM samples are signed or unsigned integers.

