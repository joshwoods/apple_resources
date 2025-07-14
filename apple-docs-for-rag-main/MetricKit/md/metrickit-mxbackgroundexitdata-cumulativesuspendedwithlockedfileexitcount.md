

- MetricKit
- MXBackgroundExitData
-  cumulativeSuspendedWithLockedFileExitCount 

Instance Property

# cumulativeSuspendedWithLockedFileExitCount

The number of times the system terminated the app from the background while being suspended and having file locks.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var cumulativeSuspendedWithLockedFileExitCount: Int { get }
```

## Discussion

A common cause for this kind of exit is writing to an SQLite database as the system is suspending the app. For information on what to do with open files and databases when transitioning to the background, see Preparing your UI to run in the background.

## See Also

### Reading the System Termination Count

var cumulativeAppWatchdogExitCount: Int

The number of times the system watchdog terminated the app from the background.

var cumulativeCPUResourceLimitExitCount: Int

The number of times the system terminated the app from the background for using too much CPU time.

var cumulativeMemoryResourceLimitExitCount: Int

The number of times the system terminated the app from the background for using too much memory.

var cumulativeMemoryPressureExitCount: Int

The number of times the system terminated the app from the background to free up memory.

