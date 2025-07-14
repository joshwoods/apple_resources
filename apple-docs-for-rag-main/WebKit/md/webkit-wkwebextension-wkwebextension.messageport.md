

- WebKit
- WKWebExtension
-  WKWebExtension.MessagePort 

Class

# WKWebExtension.MessagePort

An object that manages message-based communication with a web extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class MessagePort
```

## Overview

Contains properties and methods to handle message exchanges with a web extension.

## Topics

### Structures

struct Error

Constants that indicate errors in the WKWebExtension.MessagePort domain.

### Instance Properties

var applicationIdentifier: String?

The unique identifier for the app to which this port should be connected.

var disconnectHandler: (((any Error)?) -> Void)?

The block to be executed when the port disconnects.

var isDisconnected: Bool

Indicates whether the message port is disconnected.

var messageHandler: ((Any?, (any Error)?) -> Void)?

The block to be executed when a message is received from the web extension.

### Instance Methods

func disconnect()

Disconnects the port, terminating all further messages.

func disconnect(throwing: (any Error)?)

Disconnects the port, terminating all further messages with an optional error.

func sendMessage(Any?, completionHandler: (((any Error)?) -> Void)?)

Sends a message to the connected web extension.

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
- Sendable

## See Also

### Classes

class Action

An object that encapsulates the properties for an individual web extension action.

class Command

An object that encapsulates the properties for an individual web extension command.

class DataRecord

An object that represents a record of stored data for a specific web extension context.

class MatchPattern

An object that represents a way to specify groups of URLs.

class TabConfiguration

An object that encapsulates configuration options for a tab in an extension.

class WindowConfiguration

An object that encapsulates configuration options for a window in an extension.

class Configuration

A WKWebExtensionController.Configuration object with which to initialize a web extension controller.

