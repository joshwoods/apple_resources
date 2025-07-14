

- UIKit
-  UISmartReplySuggestion 

Class

# UISmartReplySuggestion

A class you use to handle a Smart Reply suggestion.

iOS 18.4+iPadOS 18.4+

``` source
class UISmartReplySuggestion
```

## Overview

Use the smartReply string as a signal of the user’s intention when you generate long form text based on the option the user selected.

## Topics

### Getting the Smart Reply

var smartReply: String

A string from the Smart Reply option the user selected.

## Relationships

### Inherits From

- UIInputSuggestion

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

class MessageEntry

A class that represents a message in a message conversation.

class UIInputSuggestion

A base class you use to handle suggestions from the keyboard or system.

