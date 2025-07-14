

- Message UI
-  MessageComposeResult 

Enumeration

# MessageComposeResult

These constants describe the result of the message-composition interface.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum MessageComposeResult
```

## Topics

### Constants

case cancelled

The user canceled the composition.

case sent

The user successfully queued or sent the message.

case failed

The user’s attempt to save or send the message was unsuccessful.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Responding to the Message Completion

func messageComposeViewController(MFMessageComposeViewController, didFinishWith: MessageComposeResult)

Tells the delegate that the user finished composing the message.

**Required**

