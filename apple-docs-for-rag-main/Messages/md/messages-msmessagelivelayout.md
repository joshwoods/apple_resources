

- Messages
-  MSMessageLiveLayout 

Class

# MSMessageLiveLayout

A layout that provides a custom, interactive view inside the transcript.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class MSMessageLiveLayout
```

## Overview

Use a live layout instance to create custom, interactive messages in the transcript (or input field). An alternative layout is required to represent your message on devices that don’t have your iMessage app installed, or on devices that aren’t running iOS 11 or later. Note: this could be either the receiver’s or the sender’s device; the sender may have a second device that doesn’t have your app installed.

Set the alternative layout when you instantiate your MSMessageLiveLayout object. Use an MSMessageTemplateLayout instance. The template layout automatically provides support for devices that do not support iMessage apps (macOS, iOS 9 and earlier, and SMS devices). See below for an example.

Listing 1. Sending a live message.

```
let alternateMessageLayout = MSMessageTemplateLayout()
// Configure the template layout here...

let messageLayout = MSMessageLiveLayout(alternateLayout: alternateMessageLayout)

let message = MSMessage()
message.layout = messageLayout

conversation.send(message) { (errorOrNil) in
    if let error = errorOrNil {
        // Handle the error here...
    }
}
```

When an MSMessage object with a live layout is added to the transcript (or input field), the system instantiates a new instance of your MSMessagesAppViewController subclass, with its presentationStyle property set to the MSMessagesAppPresentationStyle.transcript value.

The view controller’s selectedMessage property is set to the interactive message just before the controller’s willBecomeActive(with:) method is called. Use the selectedMessage property to access the message and display its contents.

The Messages app renders your controller’s view inside a bubble in the transcript. Your controller must check its presentation style and display an appropriate user interface for the message. You can define the message’s size by overriding your view controller’s contentSizeThatFits(_:) method.

There can be multiple live messages (from multiple iMessage apps) in the transcript at the same time. This means your app may have multiple instances of its MSMessagesAppViewController subclass running concurrently:

- One instance for each message in the transcript

- One instance for a message in the input field (when you stage the message by calling insert(_:completionHandler:))

- One instance for the app’s main interface if your iMessage app is currently active

## Topics

### Creating Live Layouts

init(alternateLayout: MSMessageTemplateLayout)

Initializes a new live layout using the provided alternate layout.

### Accessing Properties

var alternateLayout: MSMessageTemplateLayout

A template layout to be displayed when the live layout is unavailable.

## Relationships

### Inherits From

- MSMessageLayout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Interactive messages

class MSMessage

A custom message object.

class MSSession

A session object used to create and update messages.

class MSMessageLayout

An abstract base class that defines the appearance of MSMessage objects in the conversation transcript.

class MSMessageTemplateLayout

A template-based layout for custom messages.

