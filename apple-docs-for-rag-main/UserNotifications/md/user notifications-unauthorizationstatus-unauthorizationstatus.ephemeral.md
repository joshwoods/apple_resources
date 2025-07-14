

- User Notifications
- UNAuthorizationStatus
-  UNAuthorizationStatus.ephemeral 

Case

# UNAuthorizationStatus.ephemeral

The app is authorized to schedule or receive notifications for a limited amount of time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
case ephemeral
```

## Discussion

An App Clip may have the ability to schedule or receive notifications for a limited amount of time. For more information, see Enabling notifications in App Clips.

## See Also

### Status

case notDetermined

The user hasn’t yet made a choice about whether the app is allowed to schedule notifications.

case denied

The app isn’t authorized to schedule or receive notifications.

case authorized

The app is authorized to schedule or receive notifications.

case provisional

The application is provisionally authorized to post noninterruptive user notifications.

