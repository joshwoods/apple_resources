

- MetricKit
- MXBackgroundExitData
-  cumulativeBadAccessExitCount 

Instance Property

# cumulativeBadAccessExitCount

The number of times the system terminated the app from the background for attempting an invalid memory access.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var cumulativeBadAccessExitCount: Int { get }
```

## Discussion

The most common reasons for this kind of termination are an attempt to access a nonexistent or reserved memory location, or to access memory in a way that’s inconsistent with the protection level, such as writing to read-only memory.

## See Also

### Reading the Crash Count

var cumulativeIllegalInstructionExitCount: Int

The number of times the system terminated the app from the background for attempting to execute an illegal or undefined instruction.

