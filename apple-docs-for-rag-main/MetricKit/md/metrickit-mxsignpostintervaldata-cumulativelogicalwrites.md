

- MetricKit
- MXSignpostIntervalData
-  cumulativeLogicalWrites 

Instance Property

# cumulativeLogicalWrites

The total amount of data written to disk or other long term storage during the logged intervals.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var cumulativeLogicalWrites: Measurement? { get }
```

## See Also

### Reading Power and Performance Information

var averageMemory: MXAverage&lt;UnitInformationStorage>?

The average memory used during the logged intervals.

var cumulativeCPUTime: Measurement&lt;UnitDuration>?

The total amount of CPU time used during the logged intervals.

var cumulativeHitchTimeRatio: Measurement&lt;Unit>?

The ratio of the total time spent hitching to the total time spent animating during the logged intervals.

