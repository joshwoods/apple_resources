

- Messages
-  MSCriticalMessagingAuthorizationStatus 

Enumeration

# MSCriticalMessagingAuthorizationStatus

Values that describe the authorization status for the Critical Messaging API.

iOS 18.2+iPadOS 18.2+

``` source
enum MSCriticalMessagingAuthorizationStatus
```

## Topics

### Authorization statuses

case unknown

The authorization status is unknown.

case denied

A person has denied permission to use the Critical Messaging API.

case approved

A person has approved a request to use the Critical Messaging API.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Critical messages

Sending SMS messages from an app

Send critical messages from inside your app using the Critical Messaging API.

class MSCriticalSMSMessenger

The user interface for the Critical Messaging API.

struct MSRecipient

A structure that describes the recipient of a critical message.

struct MSCriticalMessage

MSCriticalMessage A simple struct to encapsulate the message string.

