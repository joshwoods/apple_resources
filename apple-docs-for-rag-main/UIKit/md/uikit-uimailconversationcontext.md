

- UIKit
-  UIMailConversationContext 

Class

# UIMailConversationContext

A class that represents an email conversation.

iOS 18.4+iPadOS 18.4+

``` source
class UIMailConversationContext
```

## Mentioned in 

Adopting Smart Reply in your messaging or email app

## Topics

### Getting message details

var responseSubject: String

A string that contains the subject line of an intended response.

var responseHasCustomSignature: Bool

A Boolean value that indicates whether the intended response contains a custom signature.

var responseSecondaryRecipientIdentifiers: Set&lt;String>

A set of strings that identifies the secondary recipients of the message, such as those in CC or BCC messages.

## Relationships

### Inherits From

- UIConversationContext

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

