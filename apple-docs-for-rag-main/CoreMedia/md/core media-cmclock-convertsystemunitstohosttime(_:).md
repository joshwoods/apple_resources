

- Core Media
- CMClock
-  convertSystemUnitsToHostTime(\_:) 

Type Method

# convertSystemUnitsToHostTime(\_:)

Converts a host time from native units to a time structure.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func convertSystemUnitsToHostTime(_ systemUnits: UInt64) -> CMTime
```

## Parameters 

`systemUnits`  

The host time to convert.

## See Also

### Converting Time

static func convertHostTimeToSystemUnits(CMTime) -> UInt64

Converts a host time from a time structure to the host time’s native units.

