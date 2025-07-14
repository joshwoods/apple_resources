

- Messages
-  MSCriticalMessagingError 

Enumeration

# MSCriticalMessagingError

Values that describe errors the Critical Messaging API returns.

iOS 18.2+iPadOS 18.2+

``` source
enum MSCriticalMessagingError
```

## Topics

### Error codes

case unknown

The error code the framework returns after an unknown error occurs.

case invalidAuthenticationRequest

The authentication request isn’t valid.

case notSupported

The framework doesn’t support the current device.

case notAuthorized

The operation isn’t authorized.

case sendFailed

The message failed to send.

## Relationships

### Conforms To

- Copyable
- CustomNSError
- Equatable
- Error
- Hashable
- LocalizedError
- RawRepresentable
- Sendable

## See Also

### Errors

let MSStickersErrorDomain: String

The error domain for stickers.

let MSMessagesErrorDomain: String

The error domain for iMessage apps.

enum MSMessageErrorCode

The error codes that the Messages framework generates.

