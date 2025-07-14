

- CallKit
- CXErrorCodeNotificationServiceExtensionError
-  missingNotificationFilteringEntitlement 

Type Property

# missingNotificationFilteringEntitlement

An error indicating that the notification service extension is missing the required filtering entitlement.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+watchOS 9.0+

``` source
static var missingNotificationFilteringEntitlement: CXErrorCodeNotificationServiceExtensionError.Code { get }
```

## Discussion

To call the reportNewIncomingVoIPPushPayload(_:completion:) method, a notification service extension must have a `com.apple.developer.usernotifications.filtering` entitlement. To apply for this entitlement, see https://developer.apple.com/contact/request/notification-service.

After you receive permission to use the entitlement, add com.apple.developer.usernotifications.filtering to the entitlements file for the Notification Service Extension target.

## See Also

### Understanding Error Codes

static var invalidClientProcess: CXErrorCodeNotificationServiceExtensionError.Code

An error indicating that an invalid client process reported the incoming call.

static var unknown: CXErrorCodeNotificationServiceExtensionError.Code

An error that occurs when there is an unknown problem.

enum Code

Constants for errors returned when reporting new, incoming VoIP calls.

