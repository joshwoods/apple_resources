

- UIKit
-  UIConversationContext 

Class

# UIConversationContext

A base class that represents a conversation between participants, such as in an email or messaging app.

iOS 18.4+iPadOS 18.4+

``` source
class UIConversationContext
```

## Topics

### Identifying the conversation

var threadIdentifier: String

A string that uniquely identifies a conversation. This identifier is persistent for the life of the conversation.

### Getting messages from the conversation

var entries: [UIConversationContext.Entry]

An array of messages in the conversation.

### Getting conversation participants

var selfIdentifiers: Set&lt;String>

A set of strings that identifies the active person in the conversation on the current device.

var responsePrimaryRecipientIdentifiers: Set&lt;String>

A dictionary that relates participant identifiers to participant names.

var participantNameByIdentifier: [String : PersonNameComponents]

A dictionary that relates participant identifiers to participant names.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIMailConversationContext
- UIMessageConversationContext

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

class Entry

A base class that represents a message in a conversation.

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

