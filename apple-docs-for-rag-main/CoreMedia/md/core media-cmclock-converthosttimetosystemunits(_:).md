

- Core Media
- CMClock
-  convertHostTimeToSystemUnits(\_:) 

Type Method

# convertHostTimeToSystemUnits(\_:)

Converts a host time from a time structure to the host time’s native units.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func convertHostTimeToSystemUnits(_ hostTime: CMTime) -> UInt64
```

## Parameters 

`hostTime`  

The host time to convert.

## See Also

### Converting Time

static func convertSystemUnitsToHostTime(UInt64) -> CMTime

Converts a host time from native units to a time structure.

