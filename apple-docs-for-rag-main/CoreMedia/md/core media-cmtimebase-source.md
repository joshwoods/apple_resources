

- Core Media
- CMTimebase
-  source 

Instance Property

# source

The immediate source that represents the clock or timebase.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var source: any CMSyncProtocol { get set }
```

## See Also

### Inspecting Timebases

var time: CMTime

The current time.

var rate: Double

The current rate relative to its immediate primary clock or timebase.

var sourceClock: CMClock?

Returns the immediate source clock, if any.

var sourceTimebase: CMTimebase?

Returns the immediate source timebase, if any.

var effectiveRate: Double

The effective rate that combines its rate with the rates of all its primary timebases.

var timeAndRate: (time: CMTime, rate: Double)

Returns the current time and rate.

var ultimateSourceClock: CMClock

Returns the source clock that’s the source of all the other source timebases.

