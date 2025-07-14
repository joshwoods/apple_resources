

- Core Media
- CMTimebase
-  rate 

Instance Property

# rate

The current rate relative to its immediate primary clock or timebase.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var rate: Double { get }
```

## See Also

### Inspecting Timebases

var time: CMTime

The current time.

var source: any CMSyncProtocol

The immediate source that represents the clock or timebase.

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

