

- UIKit
- Keyboards and input
-  Adopting Smart Reply in your messaging or email app 

Article

# Adopting Smart Reply in your messaging or email app

Generate reply suggestions by using Apple Intelligence and put selected text into your text UI.

## Overview

Messages and Mail use Apple Intelligence to provide the Smart Reply feature, which generates suggestions that are contextually relevant for a thread when you draft a message or email. To add this feature to your messaging or email app, follow these steps:

- Create a *conversation context* object with your app’s data from a thread.

- Attach the conversation context to your text view or text field when you prepare your user interface.

- Implement delegate methods to keep the conversation context up-to-date when you send or receive messages.

- For an email or other long-form type of messaging, use the selected input suggestion to generate a long-form response and place it in the entry field.

### Create a conversation context

To give Apple Intelligence the context it needs for Smart Reply generation, create a conversation context object with information about your messaging conversation. This object includes information about participants in the conversation and text entries from the conversation.

When you prepare your user interface to send and receive messages with one or more participants, create a conversation context that reflects the type of messaging thread in your app: use UIMessageConversationContext for messaging, and UIMailConversationContext for email.

Configure the conversation context with these details:

- A unique identifier for the thread

- A dictionary of unique identifiers and names of the participants in the thread

- A set of identifiers for the current person using your app to send and receive messages

- A set of identifiers for the other people in the conversation

- An array of conversation entries for the type of thread, either UIMessageConversationContext.MessageEntry or UIMailConversationContext.MailEntry

Here’s how you configure a conversation context:

- Swift
- Objective-C

```
func mailConversationContext(for yourEntries: [YourMailEntry]) -> UIMailConversationContext {
    var context: UIMailConversationContext = UIMailConversationContext()

    var contextEntries: [UIMailConversationContext.MailEntry] = []
    for yourEntry in yourEntries {
        var conversationEntry = UIMailConversationContext.MailEntry()

        conversationEntry.text = yourEntry.text
        conversationEntry.senderIdentifier = yourEntry.sender
        conversationEntry.primaryRecipientIdentifiers = [yourEntry.recipient]
        conversationEntry.sentDate = yourEntry.date
        conversationEntry.entryIdentifier = yourEntry.yourEntryIdentifier
        conversationEntry.kind = .personal

        contextEntries.append(conversationEntry)
    }

    context.threadIdentifier = yourThreadObject.identifier
    context.entries = contextEntries

    var senderName = PersonNameComponents()
    senderName.givenName = "Sender's name"

    var recipientName = PersonNameComponents()
    recipientName.givenName = "Recipient's name"

    context.participantNameByIdentifier = [senderIdentifier:senderName, recipientIdentifier: recipientName]

    context.selfIdentifiers = [senderIdentifier]

    context.responsePrimaryRecipientIdentifiers = [recipientIdentifier]

    return context
}
```

```
```

### Attach the conversation context to a text view or text field

When you create an entry field, such as a text view or text field, which you use to get input from the person using your app, assign the conversation context you created to the object’s conversationContext property before the keyboard appears:

- Swift
- Objective-C

```
entryField.conversationContext = context
```

```
```

The keyboard uses this context once per session for initialization. Use the steps in the next section to handle changes to the conversation during the keyboard session.

### Keep the conversation context up-to-date

Every time you send or receive a message, keep the conversation context up-to-date. Because the conversation context is tied to a keyboard session, update or regenerate the conversation context you created earlier if the focus changed from your entry field, then set the entry field’s `conversationContext` to the updated context:

- Swift
- Objective-C

```
entryField.conversationContext = context
```

```
```

Then, call conversationContext(_:didChange:) on the entry field’s `inputDelegate` to notify it that the conversation has more entries:

- Swift
- Objective-C

```
entryField.inputDelegate?.conversationContext(context, didChange: entryField)
```

```
```

### Generate long-form responses

For email or other long-form messaging apps, instead of dropping the Smart Reply response directly into the entry field, use the suggestion to generate a long-form response with your own model. To do this, implement textView(_:insertInputSuggestion:) or textField(_:insertInputSuggestion:):

- Swift
- Objective-C

```
func textField(_:UITextField, insertInputSuggestion inputSuggestion: UIInputSuggestion) {
    guard let smartReplySuggestion = inputSuggestion as? UISmartReplySuggestion else {
        return
    }

    // Call your model with smartReplySuggestion.smartReply,
    // then assign the result to your entry field's text property.
    let entryFieldText = YourModel.response(from:smartReplySuggestion.smartReply)
    entryField.text = entryFieldText
}
```

```
```

If your entry field is a custom implementation of UITextInput, call insert(_:) instead.

### Understand when the system generates Smart Reply suggestions

The system only generates Smart Reply suggestions in specific circumstances, and might not generate suggestions in all cases.

Circumstances when a messaging conversation can generate suggestions include:

- The input field is empty.

- The last message in the conversation is from the recipient, not the person sending messages.

- The preceding messages in the conversation are text (not images or emojis).

- The preceding messages are recent.

Circumstances when a mail conversation can generate suggestions include:

- The person is the direct recipient of the email, and is not in the CC or BCC list.

- The person has not already replied to the email.

- The sender and recipient of the email have different email addresses.

## See Also

### Smart Reply for messaging

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

class UISmartReplySuggestion

A class you use to handle a Smart Reply suggestion.

