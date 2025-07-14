

- MetricKit
-  MXBackgroundExitData 

Class

# MXBackgroundExitData

An object representing counts for the different types of background app exits.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class MXBackgroundExitData
```

## Topics

### Reading the Normal Exit Count

var cumulativeNormalAppExitCount: Int

The number of times the app exited normally from the background.

### Reading the Abnormal Exit Count

var cumulativeAbnormalExitCount: Int

The number of times the app exited abnormally from the background.

### Reading the System Termination Count

var cumulativeAppWatchdogExitCount: Int

The number of times the system watchdog terminated the app from the background.

var cumulativeCPUResourceLimitExitCount: Int

The number of times the system terminated the app from the background for using too much CPU time.

var cumulativeMemoryResourceLimitExitCount: Int

The number of times the system terminated the app from the background for using too much memory.

var cumulativeMemoryPressureExitCount: Int

The number of times the system terminated the app from the background to free up memory.

var cumulativeSuspendedWithLockedFileExitCount: Int

The number of times the system terminated the app from the background while being suspended and having file locks.

### Reading the Crash Count

var cumulativeBadAccessExitCount: Int

The number of times the system terminated the app from the background for attempting an invalid memory access.

var cumulativeIllegalInstructionExitCount: Int

The number of times the system terminated the app from the background for attempting to execute an illegal or undefined instruction.

### Reading the Timeout Count

var cumulativeBackgroundTaskAssertionTimeoutExitCount: Int

The number of times the system terminated the app from the background for exceeding the allocated time for a background task.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Reading the background exit data

var backgroundExitData: MXBackgroundExitData

The metrics for the background app exits.

