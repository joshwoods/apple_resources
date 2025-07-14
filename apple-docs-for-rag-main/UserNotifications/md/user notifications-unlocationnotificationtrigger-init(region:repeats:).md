

- User Notifications
- UNLocationNotificationTrigger
-  init(region:repeats:) 

Initializer

# init(region:repeats:)

Creates a location trigger using the region parameter.

iOS 10.0+iPadOS 10.0+watchOS 8.0+

``` source
convenience init(
    region: CLRegion,
    repeats: Bool
)
```

## Parameters 

`region`  

The geographic region that must be entered or exited. Use the region object to specify whether to deliver notifications on entry, on exit, or both.

`repeats`  

Specify false to deliver the notification one time. Specify true to reschedule the notification request each time the system delivers the notification.

## Return Value

A new location trigger object with the specified region.

## Discussion

If you specify `true` for the `repeats` parameter, you must explicitly remove the notification request to stop the delivery of the associated notification. Use the methods of UNUserNotificationCenter to remove notification requests that are no longer needed.

