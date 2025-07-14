

- AVFoundation
- AVAssetVariant
-  peakBitRate 

Instance Property

# peakBitRate

The peak bit rate for the variant.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@nonobjc
var peakBitRate: Double? { get }
```

## Discussion

If the variant doesn’t define a peak bit rate, the value is negative.

## See Also

### Configuring Bit Rate

var averageBitRate: Double?

The average bit rate for the variant.

