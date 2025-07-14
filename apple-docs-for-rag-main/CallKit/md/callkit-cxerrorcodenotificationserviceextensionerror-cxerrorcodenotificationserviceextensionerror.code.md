

- CallKit
- CXErrorCodeNotificationServiceExtensionError
-  CXErrorCodeNotificationServiceExtensionError.Code 

Enumeration

# CXErrorCodeNotificationServiceExtensionError.Code

Constants for errors returned when reporting new, incoming VoIP calls.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+watchOS 9.0+

``` source
enum Code
```

## Topics

### Error Codes

case invalidClientProcess

An error indicating that an invalid client process reported the incoming call.

case missingNotificationFilteringEntitlement

An error indicating that the notification service extension is missing the required filtering entitlement.

case unknown

An error that occurs when there is an unknown problem.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

