

- SensorKit
- SRDeviceUsageReport
-  webUsageByCategory 

Instance Property

# webUsageByCategory

The amount of time the user accesses domains per category.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var webUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.WebUsage]] { get }
```

## Discussion

The framework interprets the category in the same manner as displayed in Screen Time.

## See Also

### Analyzing Web Use

class WebUsage

An object that describes a user’s website usage.

