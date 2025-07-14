

- Core Media
-  CMClockGetHostTimeClock() 

Function

# CMClockGetHostTimeClock()

Returns a reference to the singleton clock that reflects the host time.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMClockGetHostTimeClock() -> CMClock
```

## Discussion

In macOS, the host time clock uses `mach_absolute_time` but returns a value with a large integer timescale (e.g. nanoseconds).

