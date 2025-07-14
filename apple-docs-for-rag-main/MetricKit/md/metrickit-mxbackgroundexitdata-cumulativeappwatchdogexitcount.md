

- MetricKit
- MXBackgroundExitData
-  cumulativeAppWatchdogExitCount 

Instance Property

# cumulativeAppWatchdogExitCount

The number of times the system watchdog terminated the app from the background.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var cumulativeAppWatchdogExitCount: Int { get }
```

## Discussion

The most common reasons the system watchdog terminates an app are taking too long to:

- Launch

- Terminate

- Respond to system events

## See Also

### Reading the System Termination Count

var cumulativeCPUResourceLimitExitCount: Int

The number of times the system terminated the app from the background for using too much CPU time.

var cumulativeMemoryResourceLimitExitCount: Int

The number of times the system terminated the app from the background for using too much memory.

var cumulativeMemoryPressureExitCount: Int

The number of times the system terminated the app from the background to free up memory.

var cumulativeSuspendedWithLockedFileExitCount: Int

The number of times the system terminated the app from the background while being suspended and having file locks.

