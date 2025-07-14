

- Messages
-  MSConversation 

Class

# MSConversation

An object that represents a conversation in the Messages app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
class MSConversation
```

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Overview

The MSConversation class represents a conversation in the Messages app. Use conversation objects to access information about the currently selected message or the conversation participants, or to send text, stickers, attachments, or message objects.

## Topics

### Accessing the Selected Message

var selectedMessage: MSMessage?

The message that the user selected in the conversation transcript.

### Accessing Participants

var localParticipantIdentifier: UUID

A UUID that identifies the user on this device.

var remoteParticipantIdentifiers: [UUID]

An array of UUIDs representing the remote participants in this conversation.

### Inserting Content into the Input Field

func insertAttachment(URL, withAlternateFilename: String?, completionHandler: (((any Error)?) -> Void)?)

Inserts an attachment into the current context.

func insert(MSMessage, completionHandler: (((any Error)?) -> Void)?)

Inserts a message object into the Messages app’s input field.

func insert(MSSticker, completionHandler: (((any Error)?) -> Void)?)

Inserts a sticker into the current context.

func insertText(String, completionHandler: (((any Error)?) -> Void)?)

Inserts text into the Messages app’s input field.

### Directly Sending a Message

func sendAttachment(URL, withAlternateFilename: String?, completionHandler: (((any Error)?) -> Void)?)

Sends the media file specified by the given URL.

func send(MSMessage, completionHandler: (((any Error)?) -> Void)?)

Sends a message object.

func send(MSSticker, completionHandler: (((any Error)?) -> Void)?)

Sends a sticker.

func sendText(String, completionHandler: (((any Error)?) -> Void)?)

Sends a text message.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Message content

class MSSticker

A sticker that can be sent as a new message or attached to an existing balloon in the Messages app’s transcript.

