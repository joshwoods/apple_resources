

- StoreKit
- Message
-  messages 

Type Property

# messages

The asynchronous sequence that sends a message when the App Store creates it.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
static var messages: Message.Messages { get }
```

## Mentioned in 

Testing failing subscription renewals and In-App Purchases

Merchandising win-back offers in your app

## Discussion

If your app doesn’t implement this message listener, StoreKit retrieves any messages from the App Store each time your app launches, and presents them by default.

For more information about listening for and displaying messages, see Message.

## See Also

### Getting messages and message reasons

let reason: Message.Reason

The reason that the App Store sends the message.

struct Messages

An asynchronous sequence of messages from the App Store.

struct Reason

Reasons for the App Store messages.

