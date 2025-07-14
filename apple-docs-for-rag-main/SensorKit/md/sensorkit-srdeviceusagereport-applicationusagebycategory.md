

- SensorKit
- SRDeviceUsageReport
-  applicationUsageByCategory 

Instance Property

# applicationUsageByCategory

The usage time of apps per category.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var applicationUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.ApplicationUsage]] { get }
```

## Discussion

The framework interprets the category using the primary genre an app supplies in its `iTunesMetadata.plist`.

## See Also

### Analyzing App Use

class ApplicationUsage

An object that describes the user’s app activity over a period of time.

struct CategoryKey

Categories of apps or websites that the user uses.

