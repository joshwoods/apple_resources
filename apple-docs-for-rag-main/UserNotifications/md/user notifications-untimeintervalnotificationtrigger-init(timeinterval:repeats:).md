

- User Notifications
- UNTimeIntervalNotificationTrigger
-  init(timeInterval:repeats:) 

Initializer

# init(timeInterval:repeats:)

Creates a time interval trigger using the time value parameter.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(
    timeInterval: TimeInterval,
    repeats: Bool
)
```

## Parameters 

`timeInterval`  

The time (in seconds) that must elapse from the current time before the trigger fires. This value must be greater than zero.

`repeats`  

Specify false to deliver the notification one time. Specify true to reschedule the notification request each time the system delivers the notification. If this parameter is true, the value in the `timeInterval` parameter must be 60 seconds or greater.

## Return Value

A new time interval trigger based on the specified temporal information.

## Discussion

If you specify `true` for the `repeats` parameter, you must explicitly remove the notification request to stop the delivery of the associated notification. Use the methods of UNUserNotificationCenter to remove notification requests that are no longer needed.

