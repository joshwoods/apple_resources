

- UIKit
- UIMailConversationContext
-  UIMailConversationContext.MailEntry 

Class

# UIMailConversationContext.MailEntry

A class that represents a specific email in an email thread.

iOS 18.4+iPadOS 18.4+

``` source
class MailEntry
```

## Mentioned in 

Adopting Smart Reply in your messaging or email app

## Topics

### Categorizing the email

var kind: UIMailConversationContext.MailEntry.Kind

An item that reflects the category that describes an email.

enum Kind

A set of categories for an email.

### Identifying secondary recipients

var responseSecondaryRecipientIdentifiers: Set&lt;String>

A set of strings that identifies the secondary recipients of the message, such as those in CC or BCC messages.

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

class UIMessageConversationContext

A class that represents a message conversation.

class MessageEntry

A class that represents a message in a message conversation.

class UIInputSuggestion

A base class you use to handle suggestions from the keyboard or system.

class UISmartReplySuggestion

A class you use to handle a Smart Reply suggestion.

