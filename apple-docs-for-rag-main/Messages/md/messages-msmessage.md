

- Messages
-  MSMessage 

Class

# MSMessage

A custom message object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
class MSMessage
```

## Overview

Use the MSMessage class to create custom message objects. To create interactive messages that can be updated by the conversation’s participants, instantiate a message with a session using the init(session:) method. Otherwise, instantiate the message using the init() method.

## Topics

### Creating Messages

init()

Initializes a new message that is not part of a session.

init(session: MSSession)

Initializes a new message that is part of the provided session.

### Message Properties

var accessibilityLabel: String?

A localized string that describes the message.

var error: (any Error)?

An error object describing why the system failed to send the message.

var isPending: Bool

A Boolean value that indicates whether the message is pending or whether it has been sent or received.

var layout: MSMessageLayout?

A layout object that defines the message’s appearance.

var senderParticipantIdentifier: UUID

A UUID identifying the participant that sent the message.

var session: MSSession?

The session that this message belongs to.

var shouldExpire: Bool

A Boolean value that determines whether the message should expire after being read.

var summaryText: String?

A succinct description of the message.

var url: URL?

A URL that encodes data to be transmitted with the message.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Interactive messages

class MSSession

A session object used to create and update messages.

class MSMessageLayout

An abstract base class that defines the appearance of MSMessage objects in the conversation transcript.

class MSMessageTemplateLayout

A template-based layout for custom messages.

class MSMessageLiveLayout

A layout that provides a custom, interactive view inside the transcript.

