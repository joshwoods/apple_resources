

- Core Media
- CMTime
-  epoch 

Instance Property

# epoch

The epoch of the time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
var epoch: CMTimeEpoch
```

## Discussion

Use the epoch to differentiate between equal timestamps that are different due to looping, multi-item sequencing, and so on.

## See Also

### Accessing Time Values

var value: CMTimeValue

A time value that represents the numerator of a rational time.

var timescale: CMTimeScale

A timescale that represents the denominator of a rational time.

var flags: CMTimeFlags

The flags associated with a time.

