

- AppKit
- NSHapticFeedbackManager
- NSHapticFeedbackManager.PerformanceTime
-  NSHapticFeedbackManager.PerformanceTime.now 

Case

# NSHapticFeedbackManager.PerformanceTime.now

Instructs the system to provide immediate haptic feedback to the user, rather than waiting for synchronization to occur with something visual occurring on screen.

macOS 10.11+

``` source
case now
```

## See Also

### Constants

case `default`

Allows the system to choose the most appropriate time for feedback to be provided. Currently, this is the next time the screen is updated.

case drawCompleted

Instructs the system to provide haptic feedback to the user the next time the screen is updated.

