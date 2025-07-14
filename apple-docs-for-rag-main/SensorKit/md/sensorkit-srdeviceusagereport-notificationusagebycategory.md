

- SensorKit
- SRDeviceUsageReport
-  notificationUsageByCategory 

Instance Property

# notificationUsageByCategory

The frequency of notifications per category.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var notificationUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.NotificationUsage]] { get }
```

## Discussion

The framework interprets the category using the primary genre an app supplies in its `iTunesMetadata.plist`.

## See Also

### Analyzing Notification Use

class NotificationUsage

An object that describes notification frequency and the manner in which the user interacts with notifications.

