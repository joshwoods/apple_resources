

- MetricKit
- MXBackgroundExitData
-  cumulativeMemoryPressureExitCount 

Instance Property

# cumulativeMemoryPressureExitCount

The number of times the system terminated the app from the background to free up memory.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var cumulativeMemoryPressureExitCount: Int { get }
```

## See Also

### Reading the System Termination Count

var cumulativeAppWatchdogExitCount: Int

The number of times the system watchdog terminated the app from the background.

var cumulativeCPUResourceLimitExitCount: Int

The number of times the system terminated the app from the background for using too much CPU time.

var cumulativeMemoryResourceLimitExitCount: Int

The number of times the system terminated the app from the background for using too much memory.

var cumulativeSuspendedWithLockedFileExitCount: Int

The number of times the system terminated the app from the background while being suspended and having file locks.

