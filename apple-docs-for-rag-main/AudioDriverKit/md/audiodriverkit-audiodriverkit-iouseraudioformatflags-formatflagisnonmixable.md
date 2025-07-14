

- AudioDriverKit
- AudioDriverKit
- IOUserAudioFormatFlags
-  FormatFlagIsNonMixable 

Enumeration Case

# FormatFlagIsNonMixable

A flag to indicate whether the format can’t mix.

DriverKit 21.0+

``` source
FormatFlagIsNonMixable
```

## Discussion

This flag is for use only when interacting with the Core Audio HAL’s stream format information. It isn’t a valid flag for any other uses.

## See Also

### Mixability Flags

LinearPCMFormatFlagIsNonMixable

A flag to indicate whether the PCM format can’t mix.

