

- UIKit
- UILocalNotification
-  soundName Deprecated

Instance Property

# soundName

The name of the file containing the sound to play when an alert is displayed.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var soundName: String? { get set }
```

## Discussion

For this property, specify the filename (including extension) of a sound resource in the app’s main bundle or UILocalNotificationDefaultSoundName to request the default system sound. When the system displays an alert for a local notification or badges an app icon, it plays this sound. The default value is `nil` (no sound). Sounds that last longer than 30 seconds are not supported. If you specify a file with a sound that plays over 30 seconds, the default sound is played instead.

For information on valid sound resources, see Registering, Scheduling, and Handling User Notifications in Local and Remote Notification Programming Guide.

## See Also

### Configuring other parts of the notification

var applicationIconBadgeNumber: Int

The number to display as the app’s icon badge.

Deprecated

var userInfo: [AnyHashable : Any]?

A dictionary for passing custom information to the notified app.

Deprecated

