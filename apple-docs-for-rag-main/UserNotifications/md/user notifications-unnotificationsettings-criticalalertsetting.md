

- User Notifications
- UNNotificationSettings
-  criticalAlertSetting 

Instance Property

# criticalAlertSetting

The authorization status for playing sounds for critical alerts.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 5.0+

``` source
var criticalAlertSetting: UNNotificationSetting { get }
```

## Discussion

When UNNotificationSetting.enabled, this property authorizes the app to play critical sounds that ignore Do Not Disturb and the device’s mute switch.

For local notifications, the system attempts to play a critical sound when the sound property of the UNNotificationContent object contains an object returned by the defaultCritical property, the criticalSoundNamed(_:) method, or a related method.

For remote notifications, the system attempts to play a critical sound when the notification’s payload contains a `sound` directory that contains the `critical` key.

Critical alerts require a special entitlement issued by Apple.

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

var soundSetting: UNNotificationSetting

The authorization status for playing sounds for incoming notifications.

var announcementSetting: UNNotificationSetting

The setting that indicates whether Siri can announce your app’s notifications.

var scheduledDeliverySetting: UNNotificationSetting

The setting that indicates the system schedules the notification.

var timeSensitiveSetting: UNNotificationSetting

The setting that indicates the system treats the notification as time-sensitive.

enum UNNotificationSetting

Constants that indicate the current status of a notification setting.

