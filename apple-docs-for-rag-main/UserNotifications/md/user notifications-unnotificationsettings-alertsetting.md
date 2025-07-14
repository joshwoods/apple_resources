

- User Notifications
- UNNotificationSettings
-  alertSetting 

Instance Property

# alertSetting

The authorization status for displaying alerts.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var alertSetting: UNNotificationSetting { get }
```

## Discussion

When the value of this property is UNNotificationSetting.enabled, the app is authorized to display alerts. Authorization does not guarantee that alerts always appear on the user’s screen. When a device is unlocked, the alertStyle property determines the presentation style for the alert, which can include not displaying the alert at all.

The system tries to display an alert when the title, subtitle, or body properties of a UNNotificationContent object contain values, or when the `aps` dictionary in a remote notification contains the `alert` key.

## See Also

### Getting Device-Specific Settings

var notificationCenterSetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear in Notification Center.

var lockScreenSetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear on a device’s Lock screen.

var carPlaySetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear in CarPlay.

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

