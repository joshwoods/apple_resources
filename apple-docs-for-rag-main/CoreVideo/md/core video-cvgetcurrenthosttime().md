

- Core Video
-  CVGetCurrentHostTime() 

Function

# CVGetCurrentHostTime()

Returns the current system time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+

``` source
func CVGetCurrentHostTime() -> UInt64
```

## Return Value

The current host time.

## Discussion

In macOS, the host time bases for Core Video and CoreAudio are identical—both are based on the `mach_absolute_time` function—so the values returned from either API can be used interchangeably.

## See Also

### Inspecting the Host Clock

func CVGetHostClockFrequency() -> Double

Returns the frequency of updates to the system time.

func CVGetHostClockMinimumTimeDelta() -> UInt32

Returns the smallest possible increment in the system time.

