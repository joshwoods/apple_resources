

- UIKit
- UIMessageConversationContext
-  UIMessageConversationContext.MessageEntry 

Class

# UIMessageConversationContext.MessageEntry

A class that represents a message in a message conversation.

iOS 18.4+iPadOS 18.4+

``` source
class MessageEntry
```

## Mentioned in 

Adopting Smart Reply in your messaging or email app

## Topics

### Categorizing the entry

var dataKind: UIMessageConversationContext.MessageEntry.DataKind

An item that represents the kind of data the message contains.

enum DataKind

A list of options that represent the kinds of data a message can contain.

var wasSentBySelf: Bool

A Boolean value that indicates whether the current user sent the message.

## Relationships

### Inherits From

- UIConversationContext.Entry

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

class Entry

A base class that represents a message in a conversation.

class UIMailConversationContext

A class that represents an email conversation.

class MailEntry

A class that represents a specific email in an email thread.

class UIMessageConversationContext

A class that represents a message conversation.

class UIInputSuggestion

A base class you use to handle suggestions from the keyboard or system.

class UISmartReplySuggestion

A class you use to handle a Smart Reply suggestion.

