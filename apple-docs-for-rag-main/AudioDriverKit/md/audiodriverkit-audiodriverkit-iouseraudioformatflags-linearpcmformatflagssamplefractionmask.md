

- AudioDriverKit
- AudioDriverKit
- IOUserAudioFormatFlags
-  LinearPCMFormatFlagsSampleFractionMask 

Enumeration Case

# LinearPCMFormatFlagsSampleFractionMask

A constant that indicates the bit position of a bit field within the flags, for use with fixed-point values.

DriverKit 21.0+

``` source
LinearPCMFormatFlagsSampleFractionMask
```

## Discussion

The linear PCM flags contain a 6-bit bitfield indicating that the framework should interpret an integer format as fixed point. The value indicates the number of bits used to represent the fractional portion of each sample value. This constant indicates the bit position (counting from the right) of the bitfield in the format flags.

## See Also

### Sample Fraction Flags

LinearPCMFormatFlagsSampleFractionShift

A mask used to calculate the number of fractional bits in the flags field.

