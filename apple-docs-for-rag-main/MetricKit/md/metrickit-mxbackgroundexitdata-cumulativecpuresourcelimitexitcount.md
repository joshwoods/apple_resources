

- MetricKit
- MXBackgroundExitData
-  cumulativeCPUResourceLimitExitCount 

Instance Property

# cumulativeCPUResourceLimitExitCount

The number of times the system terminated the app from the background for using too much CPU time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var cumulativeCPUResourceLimitExitCount: Int { get }
```

## See Also

### Reading the System Termination Count

var cumulativeAppWatchdogExitCount: Int

The number of times the system watchdog terminated the app from the background.

var cumulativeMemoryResourceLimitExitCount: Int

The number of times the system terminated the app from the background for using too much memory.

var cumulativeMemoryPressureExitCount: Int

The number of times the system terminated the app from the background to free up memory.

var cumulativeSuspendedWithLockedFileExitCount: Int

The number of times the system terminated the app from the background while being suspended and having file locks.

