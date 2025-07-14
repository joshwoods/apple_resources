

- UIKit
- UIConversationContext
-  UIConversationContext.Entry 

Class

# UIConversationContext.Entry

A base class that represents a message in a conversation.

iOS 18.4+iPadOS 18.4+

``` source
class Entry
```

## Topics

### Identifying the entry

var entryIdentifier: String

A string that uniquely identifies this specific entry in the conversation.

var replyThreadIdentifier: String?

An optional string that identifies another message in a conversation, when this entry is a reply to that message.

### Getting entry details

var text: String

A string that contains the message’s text.

var sentDate: Date

A date that notes when the sender added the message to the conversation.

### Identifying entry participants

var senderIdentifier: String

A string that identifies the message’s sender.

var primaryRecipientIdentifiers: Set&lt;String>

A set of strings that identifies the primary recipients of the message.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIMailConversationContext.MailEntry
- UIMessageConversationContext.MessageEntry

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Smart Reply for messaging

Adopting Smart Reply in your messaging or email app

Generate reply suggestions by using Apple Intelligence and put selected text into your text UI.

class UIConversationContext

A base class that represents a conversation between participants, such as in an email or messaging app.

class UIMailConversationContext

A class that represents an email conversation.

class MailEntry

A class that represents a specific email in an email thread.

class UIMessageConversationContext

A class that represents a message conversation.

class MessageEntry

A class that represents a message in a message conversation.

class UIInputSuggestion

A base class you use to handle suggestions from the keyboard or system.

class UISmartReplySuggestion

A class you use to handle a Smart Reply suggestion.

