

- User Notifications
- UNNotificationSettings
-  badgeSetting 

Instance Property

# badgeSetting

The setting that indicates whether badges appear on your app’s icon.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+

``` source
var badgeSetting: UNNotificationSetting { get }
```

## Discussion

When the value of this property is UNNotificationSetting.enabled, the app is authorized to badge its icon. The system tries to badge your app’s icon when the badge property of a UNNotificationContent object contain a value, or when the `aps` dictionary in a remote notification contains the `badge` key.

## See Also

### Getting Device-Specific Settings

var notificationCenterSetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear in Notification Center.

var lockScreenSetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear on a device’s Lock screen.

var carPlaySetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear in CarPlay.

var alertSetting: UNNotificationSetting

The authorization status for displaying alerts.

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

