

- MailKit
-  MEMessageActionHandler 

Protocol

# MEMessageActionHandler

An object that performs actions on messages as the system downloads them.

macOS 12.0+

``` source
protocol MEMessageActionHandler : NSObjectProtocol
```

## Overview

As MailKit downloads messages, it invokes the decideAction(for:completionHandler:) method on your handler. You indicate the action to take for each message, such as marking it as read or unread, flagging it, or archiving it.

To indicate that your extension contains a message action handler, add `MEMessageActionHandler` to the MEExtensionCapabilities array in the extension’s `Info.plist` file:

```
NSExtensionAttributes

    MEExtensionCapabilities

        MEMessageActionHandler

```

## Topics

### Performing Actions on Messages

func decideAction(for: MEMessage, completionHandler: (MEMessageActionDecision?) -> Void)

Determines the action that the system takes when it downloads a message.

**Required**

class MEMessageAction

An action the system performs on a message, such as setting a color or archiving it.

class MEMessageActionDecision

The action that the system performs on a message, or a request to ask the action handler again later when the message content is available.

enum MessageColor

A color that the system uses to display a message in the message list.

### Instance Properties

var requiredHeaders: [String]

## Relationships

### Inherits From

- NSObjectProtocol

