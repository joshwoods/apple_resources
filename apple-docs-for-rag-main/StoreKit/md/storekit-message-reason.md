

- StoreKit
- Message
-  reason 

Instance Property

# reason

The reason that the App Store sends the message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
let reason: Message.Reason
```

## See Also

### Getting messages and message reasons

static var messages: Message.Messages

The asynchronous sequence that sends a message when the App Store creates it.

struct Messages

An asynchronous sequence of messages from the App Store.

struct Reason

Reasons for the App Store messages.

