

- User Notifications
- UNNotificationSettings
-  soundSetting 

Instance Property

# soundSetting

The authorization status for playing sounds for incoming notifications.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var soundSetting: UNNotificationSetting { get }
```

## Discussion

When the value of this property is UNNotificationSetting.enabled, the system authorizes the app to play sounds. The system tries to play a sound when the sound property of the UNNotificationContent object contains a value, or when the `aps` dictionary in a remote notification contains the `sound` key.

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

var badgeSetting: UNNotificationSetting

The setting that indicates whether badges appear on your app’s icon.

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

