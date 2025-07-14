

- User Notifications
- UNNotificationRequest
-  init(identifier:content:trigger:) 

Initializer

# init(identifier:content:trigger:)

Creates a notification request object that you use to schedule a notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(
    identifier: String,
    content: UNNotificationContent,
    trigger: UNNotificationTrigger?
)
```

## Parameters 

`identifier`  

An identifier for the request; this parameter must not be `nil`. You can use this identifier to cancel the request if it’s still pending (see the removePendingNotificationRequests(withIdentifiers:) method).

`content`  

The content of the notification. This parameter must not be `nil`.

`trigger`  

The condition that causes the system to deliver the notification. Specify `nil` to deliver the notification right away.

## Return Value

A new notification request object.

## Discussion

Use this method when you want to schedule the delivery of a local notification. This method creates the request object that you subsequently pass to the add(_:withCompletionHandler:) method.

The system uses the `identifier` parameter to determine how to handle the request:

- **If you provide a unique identifier,** the system creates a new notification.

- **If the identifier matches a previously delivered notification,** the system alerts the user again, replaces the old notification with the new one, and places the new notification at the top of the list.

- **If the identifier matches a pending request,** the new request replaces the pending request.

