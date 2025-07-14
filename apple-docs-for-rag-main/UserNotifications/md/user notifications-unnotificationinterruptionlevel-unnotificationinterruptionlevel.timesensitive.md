

- User Notifications
- UNNotificationInterruptionLevel
-  UNNotificationInterruptionLevel.timeSensitive 

Case

# UNNotificationInterruptionLevel.timeSensitive

The system presents the notification immediately, lights up the screen, can play a sound, and breaks through system notification controls.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case timeSensitive
```

## Discussion

Time Sensitive notifications are similar to active notifications, but can break through system controls such as Notification Summary and Focus. The user can turn off the ability for time sensitive notification interruptions.

## See Also

### Enumeration Cases

case active

The system presents the notification immediately, lights up the screen, and can play a sound.

case critical

The system presents the notification immediately, lights up the screen, and bypasses the mute switch to play a sound.

case passive

The system adds the notification to the notification list without lighting up the screen or playing a sound.

