

- MetricKit
- MXBackgroundExitData
-  cumulativeIllegalInstructionExitCount 

Instance Property

# cumulativeIllegalInstructionExitCount

The number of times the system terminated the app from the background for attempting to execute an illegal or undefined instruction.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var cumulativeIllegalInstructionExitCount: Int { get }
```

## Discussion

One way to trigger this exit is by invoking a function with a misconfigured function pointer.

## See Also

### Reading the Crash Count

var cumulativeBadAccessExitCount: Int

The number of times the system terminated the app from the background for attempting an invalid memory access.

