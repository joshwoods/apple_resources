

- User Notifications
- UNNotificationSettings
-  carPlaySetting 

Instance Property

# carPlaySetting

The setting that indicates whether your app’s notifications appear in CarPlay.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var carPlaySetting: UNNotificationSetting { get }
```

## See Also

### Getting Device-Specific Settings

var notificationCenterSetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear in Notification Center.

var lockScreenSetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear on a device’s Lock screen.

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

