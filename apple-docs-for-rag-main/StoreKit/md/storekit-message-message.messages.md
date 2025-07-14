

- StoreKit
- Message
-  Message.Messages 

Structure

# Message.Messages

An asynchronous sequence of messages from the App Store.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
struct Messages
```

## Overview

The `Message.Messages` structure provides a sequence of messages that the App Store sends to your app. Iterate over the contents of this structure asynchronously to retrieve each message if your app needs to delay the message.

Don’t create this structure directly. Instead, use messages method to retrieve the messages.

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Getting messages and message reasons

static var messages: Message.Messages

The asynchronous sequence that sends a message when the App Store creates it.

let reason: Message.Reason

The reason that the App Store sends the message.

struct Reason

Reasons for the App Store messages.

