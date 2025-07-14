

- MetricKit
-  MXSignpostIntervalData 

Class

# MXSignpostIntervalData

A data object representing the captured data for a custom metric.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXSignpostIntervalData
```

## Topics

### Reading Histogrammed Custom Metric Durations

var histogrammedSignpostDuration: MXHistogram&lt;UnitDuration>

A histogram of the different time intervals of a custom metric event.

### Reading Power and Performance Information

var averageMemory: MXAverage&lt;UnitInformationStorage>?

The average memory used during the logged intervals.

var cumulativeCPUTime: Measurement&lt;UnitDuration>?

The total amount of CPU time used during the logged intervals.

var cumulativeLogicalWrites: Measurement&lt;UnitInformationStorage>?

The total amount of data written to disk or other long term storage during the logged intervals.

var cumulativeHitchTimeRatio: Measurement&lt;Unit>?

The ratio of the total time spent hitching to the total time spent animating during the logged intervals.

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

### Reading custom metric data

var signpostIntervalData: MXSignpostIntervalData?

The data captured for a custom metric.

