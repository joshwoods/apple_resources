

- User Notifications
- UNNotificationInterruptionLevel
-  UNNotificationInterruptionLevel.critical 

Case

# UNNotificationInterruptionLevel.critical

The system presents the notification immediately, lights up the screen, and bypasses the mute switch to play a sound.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case critical
```

## Discussion

This interruption level requires an approved entitlement. The system always presents this notification, even when Do Not Disturb is active. If your app doesn’t assign a sound to this notification, the system uses the default critical alert sound.

## See Also

### Enumeration Cases

case active

The system presents the notification immediately, lights up the screen, and can play a sound.

case passive

The system adds the notification to the notification list without lighting up the screen or playing a sound.

case timeSensitive

The system presents the notification immediately, lights up the screen, can play a sound, and breaks through system notification controls.

