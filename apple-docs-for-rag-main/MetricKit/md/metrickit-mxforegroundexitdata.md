

- MetricKit
-  MXForegroundExitData 

Class

# MXForegroundExitData

An object representing counts for the different types of foreground app exits.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class MXForegroundExitData
```

## Topics

### Reading the Normal Exit Count

var cumulativeNormalAppExitCount: Int

The number of times the app exited normally from the foreground.

### Reading the Abnormal Exit Count

var cumulativeAbnormalExitCount: Int

The number of times the app exited abnormally from the foreground.

### Reading the System Termination Count

var cumulativeAppWatchdogExitCount: Int

The number of times the system watchdog terminated the app from the foreground.

var cumulativeMemoryResourceLimitExitCount: Int

The number of times the system terminated the app from the foreground for using too much memory.

### Reading the Crash Count

var cumulativeBadAccessExitCount: Int

The number of times the system terminated the app from the foreground for attempting an invalid memory access.

var cumulativeIllegalInstructionExitCount: Int

The number of times the system terminated the app from the foreground for attempting to execute an illegal or undefined instruction.

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

### Reading the foreground exit data

var foregroundExitData: MXForegroundExitData

The metrics for the foreground app exits.

