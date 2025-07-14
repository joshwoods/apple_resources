

- WebKit
- WKWebExtensionController
-  WKWebExtensionController.Configuration 

Class

# WKWebExtensionController.Configuration

A WKWebExtensionController.Configuration object with which to initialize a web extension controller.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class Configuration
```

## Overview

Contains properties used to configure a WKWebExtensionController.

## Topics

### Initializers

convenience init(identifier: UUID)

Returns a new configuration that is persistent and unique for the specified identifier.

### Instance Properties

var defaultWebsiteDataStore: WKWebsiteDataStore!

The default data store for website data and cookie access in extension contexts.

var identifier: UUID?

The unique identifier used for persistent configuration storage, or `nil` when it is the default or not persistent.

var isPersistent: Bool

A Boolean value indicating if this context will write data to the the file system.

var webViewConfiguration: WKWebViewConfiguration!

The web view configuration to be used as a basis for configuring web views in extension contexts.

### Type Methods

class func `default`() -> Self

Returns a new default configuration that is persistent and not unique.

class func nonPersistent() -> Self

Returns a new non-persistent configuration.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
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

class WindowConfiguration

An object that encapsulates configuration options for a window in an extension.

