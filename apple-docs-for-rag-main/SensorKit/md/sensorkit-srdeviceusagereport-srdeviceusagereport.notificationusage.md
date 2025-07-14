

- SensorKit
- SRDeviceUsageReport
-  SRDeviceUsageReport.NotificationUsage 

Class

# SRDeviceUsageReport.NotificationUsage

An object that describes notification frequency and the manner in which the user interacts with notifications.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class NotificationUsage
```

## Overview

Each instance of this class represents a user notification in a particular app category. For more information, see notificationUsageByCategory.

## Topics

### Analyzing Notification Use

var bundleIdentifier: String?

The bundle identifier of the app that corresponds to the notification.

var event: SRDeviceUsageReport.NotificationUsage.Event

The way that the user interacts with the notification.

enum Event

The ways that a user interacts with notifications.

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

### Analyzing Notification Use

var notificationUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.NotificationUsage]]

The frequency of notifications per category.

