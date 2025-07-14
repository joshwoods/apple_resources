

- WebKit
- WKWebExtension
-  WKWebExtension.WindowConfiguration 

Class

# WKWebExtension.WindowConfiguration

An object that encapsulates configuration options for a window in an extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class WindowConfiguration
```

## Overview

This class holds various options that influence the behavior and initial state of a window.

The app retains the discretion to disregard any or all of these options, or even opt not to create a window.

## Topics

### Instance Properties

var frame: CGRect

Indicates the frame where the window should be positioned on the main screen.

var shouldBeFocused: Bool

Indicates whether the window should be focused.

var shouldBePrivate: Bool

Indicates whether the window should be private.

var tabURLs: [URL]

Indicates the URLs that the window should initially load as tabs.

var tabs: [any WKWebExtensionTab]

Indicates the existing tabs that should be moved to the window.

var windowState: WKWebExtension.WindowState

Indicates the window state for the window.

var windowType: WKWebExtension.WindowType

Indicates the window type for the window.

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

class MessagePort

An object that manages message-based communication with a web extension.

class TabConfiguration

An object that encapsulates configuration options for a tab in an extension.

class Configuration

A WKWebExtensionController.Configuration object with which to initialize a web extension controller.

