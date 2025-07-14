

- WebKit
- WKWebExtension
-  WKWebExtension.TabConfiguration 

Class

# WKWebExtension.TabConfiguration

An object that encapsulates configuration options for a tab in an extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class TabConfiguration
```

## Overview

This class holds various options that influence the behavior and initial state of a tab.

The app retains the discretion to disregard any or all of these options, or even opt not to create a tab.

## Topics

### Instance Properties

var index: Int

Indicates the position where the tab should be opened within the window.

var parentTab: (any WKWebExtensionTab)?

Indicates the parent tab with which the tab should be related.

var shouldAddToSelection: Bool

Indicates whether the tab should be added to the current tab selection.

var shouldBeActive: Bool

Indicates whether the tab should be the active tab.

var shouldBeMuted: Bool

Indicates whether the tab should be muted.

var shouldBePinned: Bool

Indicates whether the tab should be pinned.

var shouldReaderModeBeActive: Bool

Indicates whether reader mode in the tab should be active.

var url: URL?

Indicates the initial URL for the tab.

var window: (any WKWebExtensionWindow)?

Indicates the window where the tab should be opened.

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

class WindowConfiguration

An object that encapsulates configuration options for a window in an extension.

class Configuration

A WKWebExtensionController.Configuration object with which to initialize a web extension controller.

