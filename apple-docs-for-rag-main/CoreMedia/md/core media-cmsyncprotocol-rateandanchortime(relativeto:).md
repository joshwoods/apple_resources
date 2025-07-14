

- Core Media
- CMSyncProtocol
-  rateAndAnchorTime(relativeTo:) 

Instance Method

# rateAndAnchorTime(relativeTo:)

Queries the relative rate of one timebase or clock relative to another timebase or clock, and the times of each timebase or clock at which the relative rate went into effect.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func rateAndAnchorTime(relativeTo clockOrTimebase: T) throws -> (rate: Double, anchorTime: CMTime, referenceTime: CMTime) where T : CMSyncProtocol
```

**Required**

## Parameters 

`clockOrTimebase`  

The clock to compare to.

## See Also

### Getting the Time Rate

func rate&lt;T>(relativeTo: T) -> Double

Queries the relative rate of one timebase or clock relative to another timebase or clock.

**Required**

