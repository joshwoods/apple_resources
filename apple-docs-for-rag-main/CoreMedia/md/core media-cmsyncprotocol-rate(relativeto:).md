

- Core Media
- CMSyncProtocol
-  rate(relativeTo:) 

Instance Method

# rate(relativeTo:)

Queries the relative rate of one timebase or clock relative to another timebase or clock.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func rate(relativeTo clockOrTimebase: T) -> Double where T : CMSyncProtocol
```

**Required**

## Parameters 

`clockOrTimebase`  

The clock to compare to.

## See Also

### Getting the Time Rate

func rateAndAnchorTime&lt;T>(relativeTo: T) throws -> (rate: Double, anchorTime: CMTime, referenceTime: CMTime)

Queries the relative rate of one timebase or clock relative to another timebase or clock, and the times of each timebase or clock at which the relative rate went into effect.

**Required**

