

- Core Media
-  CMSyncProtocol 

Protocol

# CMSyncProtocol

A type that provides behavior for syncing time.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol CMSyncProtocol : Sendable
```

## Topics

### Getting the Time

var time: CMTime

The current time.

**Required**

### Converting Time

func convertTime&lt;T>(CMTime, to: T) -> CMTime

Converts a time from one timebase or clock to another timebase or clock.

**Required**

### Getting the Time Rate

func rate&lt;T>(relativeTo: T) -> Double

Queries the relative rate of one timebase or clock relative to another timebase or clock.

**Required**

func rateAndAnchorTime&lt;T>(relativeTo: T) throws -> (rate: Double, anchorTime: CMTime, referenceTime: CMTime)

Queries the relative rate of one timebase or clock relative to another timebase or clock, and the times of each timebase or clock at which the relative rate went into effect.

**Required**

### Determining Time Drift

func mightDrift&lt;T>(relativeTo: T) -> Bool

Returns a Boolean value that indicates whether it’s possible for the clock to drift relative to the input.

**Required**

## Relationships

### Inherits From

- Sendable

### Conforming Types

- CMClock
- CMTimebase

## See Also

### Data Types

class CMTimebase

A model of a timeline under application control.

struct CMSync

A type that represents time syncing.

