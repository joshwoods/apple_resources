

- CallKit
- CXErrorCodeNotificationServiceExtensionError
-  invalidClientProcess 

Type Property

# invalidClientProcess

An error indicating that an invalid client process reported the incoming call.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+watchOS 9.0+

``` source
static var invalidClientProcess: CXErrorCodeNotificationServiceExtensionError.Code { get }
```

## Discussion

Only call the reportNewIncomingVoIPPushPayload(_:completion:) method from a UNNotificationServiceExtension object that is responding to an incoming notification request.

## See Also

### Understanding Error Codes

static var missingNotificationFilteringEntitlement: CXErrorCodeNotificationServiceExtensionError.Code

An error indicating that the notification service extension is missing the required filtering entitlement.

static var unknown: CXErrorCodeNotificationServiceExtensionError.Code

An error that occurs when there is an unknown problem.

enum Code

Constants for errors returned when reporting new, incoming VoIP calls.

