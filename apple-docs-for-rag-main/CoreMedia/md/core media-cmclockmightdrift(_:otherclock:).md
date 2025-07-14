

- Core Media
-  CMClockMightDrift(\_:otherClock:) 

Function

# CMClockMightDrift(\_:otherClock:)

Returns a Boolean value that indicates whether it’s possible for two clocks to drift relative to each other.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMClockMightDrift(
    _ clock: CMClock,
    otherClock: CMClock
) -> Bool
```

## Parameters 

`clock`  

The first clock to compare.

`otherClock`  

The second clock to compare.

## See Also

### Determining Clock Drift

func CMSyncMightDrift(CMClockOrTimebase, CMClockOrTimebase) -> Bool

Returns a Boolean value that indicates whether it’s possible for one timebase or clock to drift relative to the other.

