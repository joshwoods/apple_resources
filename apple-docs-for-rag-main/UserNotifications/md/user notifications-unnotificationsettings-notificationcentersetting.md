

- User Notifications
- UNNotificationSettings
-  notificationCenterSetting 

Instance Property

# notificationCenterSetting

The setting that indicates whether your app’s notifications appear in Notification Center.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var notificationCenterSetting: UNNotificationSetting { get }
```

## Mentioned in 

Asking permission to use notifications

## Discussion

The default value of this property is UNNotificationSetting.enabled.

## See Also

### Getting Device-Specific Settings

var lockScreenSetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear on a device’s Lock screen.

var carPlaySetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear in CarPlay.

var alertSetting: UNNotificationSetting

The authorization status for displaying alerts.

var badgeSetting: UNNotificationSetting

The setting that indicates whether badges appear on your app’s icon.

var soundSetting: UNNotificationSetting

The authorization status for playing sounds for incoming notifications.

var criticalAlertSetting: UNNotificationSetting

The authorization status for playing sounds for critical alerts.

var announcementSetting: UNNotificationSetting

The setting that indicates whether Siri can announce your app’s notifications.

var scheduledDeliverySetting: UNNotificationSetting

The setting that indicates the system schedules the notification.

var timeSensitiveSetting: UNNotificationSetting

The setting that indicates the system treats the notification as time-sensitive.

enum UNNotificationSetting

Constants that indicate the current status of a notification setting.

