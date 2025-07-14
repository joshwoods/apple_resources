

- Messages
-  MSCriticalSMSMessenger 

Class

# MSCriticalSMSMessenger

The user interface for the Critical Messaging API.

iOS 18.2+iPadOS 18.2+

``` source
@objc
class MSCriticalSMSMessenger
```

## Topics

### Determining the maximum allowed recipients

var maximumCriticalMessagingRecipients: Int

An integer that defines the maximum number of recipients to which the framework can send messages at one time.

### Requesting authorization

func requestAuthorization(for: [MSRecipient]) async throws -> [MSRecipient : MSCriticalMessagingAuthorizationStatus]

Requests a person’s authorization to send messages to the provided recipients.

### Checking authorization status

func checkAuthorizationStatus(for: [MSRecipient]) async throws -> [MSRecipient : MSCriticalMessagingAuthorizationStatus]

Confirms the current authorization status for sending critical messages from this app.

### Sending critical messages

func send(MSCriticalMessage, to: MSRecipient) async throws -> Bool

Sends a critical message to the specified recipient.

### Instance Methods

init()

Creates an instance of the critical messenger object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Critical messages

Sending SMS messages from an app

Send critical messages from inside your app using the Critical Messaging API.

struct MSRecipient

A structure that describes the recipient of a critical message.

struct MSCriticalMessage

MSCriticalMessage A simple struct to encapsulate the message string.

enum MSCriticalMessagingAuthorizationStatus

Values that describe the authorization status for the Critical Messaging API.

