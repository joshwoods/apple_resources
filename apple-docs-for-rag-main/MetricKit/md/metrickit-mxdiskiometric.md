

- MetricKit
-  MXDiskIOMetric 

Class

# MXDiskIOMetric

An object representing metrics about disk usage.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXDiskIOMetric
```

## Topics

### Reading disk use

var cumulativeLogicalWrites: Measurement&lt;UnitInformationStorage>

The total amount of data written to disk or other long term storage.

## Relationships

### Inherits From

- MXMetric

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

### Disk access metrics

class MXDiskWriteExceptionDiagnostic

An object representing a diagnostic report for a disk write exception.

