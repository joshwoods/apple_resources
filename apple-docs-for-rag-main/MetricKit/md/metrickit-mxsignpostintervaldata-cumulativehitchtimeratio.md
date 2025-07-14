

- MetricKit
- MXSignpostIntervalData
-  cumulativeHitchTimeRatio 

Instance Property

# cumulativeHitchTimeRatio

The ratio of the total time spent hitching to the total time spent animating during the logged intervals.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
var cumulativeHitchTimeRatio: Measurement? { get }
```

## See Also

### Reading Power and Performance Information

var averageMemory: MXAverage&lt;UnitInformationStorage>?

The average memory used during the logged intervals.

var cumulativeCPUTime: Measurement&lt;UnitDuration>?

The total amount of CPU time used during the logged intervals.

var cumulativeLogicalWrites: Measurement&lt;UnitInformationStorage>?

The total amount of data written to disk or other long term storage during the logged intervals.

