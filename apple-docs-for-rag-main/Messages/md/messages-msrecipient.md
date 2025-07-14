

- Messages
-  MSRecipient 

Structure

# MSRecipient

A structure that describes the recipient of a critical message.

iOS 18.2+iPadOS 18.2+

``` source
struct MSRecipient
```

## Topics

### Creating recipients

init(phoneNumber: String)

Creates a new critical message recipient with the provided phone number.

### Properties

var phoneNumber: String

The phone number of a critical message recipient.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Critical messages

Sending SMS messages from an app

Send critical messages from inside your app using the Critical Messaging API.

class MSCriticalSMSMessenger

The user interface for the Critical Messaging API.

struct MSCriticalMessage

MSCriticalMessage A simple struct to encapsulate the message string.

enum MSCriticalMessagingAuthorizationStatus

Values that describe the authorization status for the Critical Messaging API.

