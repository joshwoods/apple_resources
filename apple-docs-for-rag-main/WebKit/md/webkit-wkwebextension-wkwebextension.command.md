

- WebKit
- WKWebExtension
-  WKWebExtension.Command 

Class

# WKWebExtension.Command

An object that encapsulates the properties for an individual web extension command.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class Command
```

## Overview

Provides access to command properties such as a unique identifier, a descriptive title, and shortcut keys. Commands can be used by a web extension to perform specific actions within a web extension context, such toggling features, or interacting with web content. These commands enhance the functionality of the extension by allowing users to invoke actions quickly.

## Topics

### Instance Properties

var activationKey: String?

The primary key used to trigger the command, distinct from any modifier flags.

var id: String

A unique identifier for the command.

var keyCommand: UIKeyCommand?

A key command representation of the web extension command for use in the responder chain.

var menuItem: UIMenuElement

A menu item representation of the web extension command for use in menus.

var modifierFlags: UIKeyModifierFlags

The modifier flags used with the activation key to trigger the command.

var title: String

A descriptive title for the command to help discoverability.

var webExtensionContext: WKWebExtensionContext?

The web extension context associated with the command.

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

class DataRecord

An object that represents a record of stored data for a specific web extension context.

class MatchPattern

An object that represents a way to specify groups of URLs.

class MessagePort

An object that manages message-based communication with a web extension.

class TabConfiguration

An object that encapsulates configuration options for a tab in an extension.

class WindowConfiguration

An object that encapsulates configuration options for a window in an extension.

class Configuration

A WKWebExtensionController.Configuration object with which to initialize a web extension controller.

