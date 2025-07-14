

- Bundle Resources
- Entitlements
-  com.apple.developer.usernotifications.filtering 

Property List Key

# com.apple.developer.usernotifications.filtering

Enable receiving notifications without displaying the notification to the user.

iOS 13.3+iPadOS 13.3+macOS 11.0+

## Details 

Type  

boolean

## Discussion

This entitlement allows a notification service extension to receive remote notifications without displaying the notification to the user. To apply for this entitlement, see Request Notification Service Entitlement.

After you receive permission to use the entitlement, add com.apple.developer.usernotifications.filtering to the entitlements file in the Notification Service Extension target. This allows you to silence push notifications after your extension receives them.

### Silence Push Notifications

To suppress a notification’s alert, create an empty UNNotificationContent object in your extension’s didReceive(_:withContentHandler:) method, and pass it to the content handler. Don’t specify a title, subtitle, body, attachments, or sound for the content.

```
override func didReceive(_ request: UNNotificationRequest, withContentHandler contentHandler: @escaping (UNNotificationContent) -> Void) {

    // Determine whether you should suppress the notification.
    let suppress = myShouldSuppressNotification(request: request)

    if suppress {
        // Don't deliver the notification to the user.
        contentHandler(UNNotificationContent())

    } else {
        // Deliver the notification.
        guard let updatedContent = request.content.mutableCopy() as? UNMutableNotificationContent else {
            // This error should never occur.
            fatalError("Unable to create a mutable copy of the content")
        }

        // Update the notification's content, such as decrypting the body, here. 
        contentHandler(updatedContent)
    }
}
```

Note

To silence a remote notification, you must set the `apns-push-type` header field to `alert` when you send the notification to the APNS server. Otherwise, the system always displays the notification banner to the user.

## See Also

### Notifications

APS Environment Entitlement

The environment for push notifications.

**Key:** aps-environment

APS Environment (macOS) Entitlement

The environment for push notifications in macOS apps.

**Key:** com.apple.developer.aps-environment

