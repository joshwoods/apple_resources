

- CallKit
- CXErrorCodeNotificationServiceExtensionError
- CXErrorCodeNotificationServiceExtensionError.Code
-  CXErrorCodeNotificationServiceExtensionError.Code.invalidClientProcess 

Case

# CXErrorCodeNotificationServiceExtensionError.Code.invalidClientProcess

An error indicating that an invalid client process reported the incoming call.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+watchOS 9.0+

``` source
case invalidClientProcess
```

## Discussion

Only call the reportNewIncomingVoIPPushPayload(_:completion:) method from a UNNotificationServiceExtension object that is responding to an incoming notification request.

## See Also

### Error Codes

case missingNotificationFilteringEntitlement

An error indicating that the notification service extension is missing the required filtering entitlement.

case unknown

An error that occurs when there is an unknown problem.

