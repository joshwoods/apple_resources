

- Core Media
- CMTimebase
-  setRateAndAnchorTime(rate:anchorTime:referenceTime:) 

Instance Method

# setRateAndAnchorTime(rate:anchorTime:referenceTime:)

Sets the time at a particular primary time, and changes the rate at exactly that time.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setRateAndAnchorTime(
    rate: Double,
    anchorTime: CMTime,
    referenceTime: CMTime
) throws
```

## See Also

### Getting and Setting the Timebase Rate

func setRate(Double) throws

Sets the rate.

