

- CallKit
- CXErrorCodeNotificationServiceExtensionError
- CXErrorCodeNotificationServiceExtensionError.Code
-  CXErrorCodeNotificationServiceExtensionError.Code.missingNotificationFilteringEntitlement 

Case

# CXErrorCodeNotificationServiceExtensionError.Code.missingNotificationFilteringEntitlement

An error indicating that the notification service extension is missing the required filtering entitlement.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+watchOS 9.0+

``` source
case missingNotificationFilteringEntitlement
```

## Discussion

To call the reportNewIncomingVoIPPushPayload(_:completion:) method, a notification service extension must have a `com.apple.developer.usernotifications.filtering` entitlement. To apply for this entitlement, see https://developer.apple.com/contact/request/notification-service.

After you receive permission to use the entitlement, add com.apple.developer.usernotifications.filtering to the entitlements file for the Notification Service Extension target.

## See Also

### Error Codes

case invalidClientProcess

An error indicating that an invalid client process reported the incoming call.

case unknown

An error that occurs when there is an unknown problem.

