

- SensorKit
- SRDeviceUsageReport
-  SRDeviceUsageReport.WebUsage 

Class

# SRDeviceUsageReport.WebUsage

An object that describes a user’s website usage.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class WebUsage
```

## Overview

Each instance of this class represents a website in a particular app category. For more information, see webUsageByCategory.

## Topics

### Timing Web Use

var totalUsageTime: TimeInterval

The amount of web usage time that the report spans.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Analyzing Web Use

var webUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.WebUsage]]

The amount of time the user accesses domains per category.

