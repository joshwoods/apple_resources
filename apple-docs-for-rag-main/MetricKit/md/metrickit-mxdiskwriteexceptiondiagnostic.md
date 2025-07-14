

- MetricKit
-  MXDiskWriteExceptionDiagnostic 

Class

# MXDiskWriteExceptionDiagnostic

An object representing a diagnostic report for a disk write exception.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
class MXDiskWriteExceptionDiagnostic
```

## Overview

A disk write exception occurs when the app writes an excessive amount of data to the disk.

## Topics

### Reading total disk writes

var totalWritesCaused: Measurement&lt;UnitInformationStorage>

The total amount of data written to disk or other long-term storage during the disk write exception.

### Viewing the call stack

var callStackTree: MXCallStackTree

The call stack for the disk write exception.

## Relationships

### Inherits From

- MXDiagnostic

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

class MXDiskIOMetric

An object representing metrics about disk usage.

