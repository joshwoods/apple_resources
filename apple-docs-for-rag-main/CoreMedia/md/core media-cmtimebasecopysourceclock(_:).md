

- Core Media
-  CMTimebaseCopySourceClock(\_:) 

Function

# CMTimebaseCopySourceClock(\_:)

Returns the immediate source clock of a timebase.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseCopySourceClock(_ timebase: CMTimebase) -> CMClock?
```

## See Also

### Copying Timebases

func CMTimebaseCopySource(CMTimebase) -> CMClockOrTimebase

Returns the immediate source — either a clock or timebase — of a timebase.

func CMTimebaseCopySourceTimebase(CMTimebase) -> CMTimebase?

Returns the immediate source timebase of a timebase.

func CMTimebaseCopyUltimateSourceClock(CMTimebase) -> CMClock

Returns the source clock that’s the source of all of a timebase’s source timebases.

