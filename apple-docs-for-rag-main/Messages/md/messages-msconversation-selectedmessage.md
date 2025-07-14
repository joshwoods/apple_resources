

- Messages
- MSConversation
-  selectedMessage 

Instance Property

# selectedMessage

The message that the user selected in the conversation transcript.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var selectedMessage: MSMessage? { get }
```

## Discussion

If the user selected one of your extension’s messages in the conversation transcript, this property is set to the selected message object. Otherwise, it is set to `nil`.

If your extension was launched because the user selected the message, then this property is set when the extension is launched.

If the user selects a message while your extension is running, the system takes the following steps:

1.  Invokes your MSMessagesAppViewController object’s willSelect(_:conversation:) method.

2.  Updates the conversation’s `selectedMessage` property.

3.  Invokes your MSMessagesAppViewController object’s didSelect(_:conversation:) method.

Override willSelect(_:conversation:) or didSelect(_:conversation:) to handle changes to the selected message while your extension is active.

Note

This property is always set to the message object selected by the user. If this message belongs to a session, then the selected message might not contain the most current data. The selected message is not updated when you receive new messages. Instead, override your view controller’s didReceive(_:conversation:) message to handle updates.

