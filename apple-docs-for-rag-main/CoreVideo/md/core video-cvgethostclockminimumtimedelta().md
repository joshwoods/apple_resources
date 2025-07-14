

- Core Video
-  CVGetHostClockMinimumTimeDelta() 

Function

# CVGetHostClockMinimumTimeDelta()

Returns the smallest possible increment in the system time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+

``` source
func CVGetHostClockMinimumTimeDelta() -> UInt32
```

## Return Value

The smallest valid increment in the system time.

## See Also

### Inspecting the Host Clock

func CVGetCurrentHostTime() -> UInt64

Returns the current system time.

func CVGetHostClockFrequency() -> Double

Returns the frequency of updates to the system time.

