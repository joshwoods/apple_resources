

- MetricKit
- MXCPUMetric
-  cumulativeCPUInstructions 

Instance Property

# cumulativeCPUInstructions

The total number of CPU instructions the app executed during the reporting period.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var cumulativeCPUInstructions: Measurement { get }
```

## Discussion

For CPUs using out-of-order execution, this property represents the count of instructions the pipeline fully executes. These instructions are sometimes referred to as *retired instructions*.

## See Also

### Reading CPU use

var cumulativeCPUTime: Measurement&lt;UnitDuration>

The total amount of CPU the app used.

