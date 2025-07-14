

- WebKit
- WKWebExtension
-  WKWebExtension.DataRecord 

Class

# WKWebExtension.DataRecord

An object that represents a record of stored data for a specific web extension context.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class DataRecord
```

## Overview

Contains properties and methods to query the data types and sizes.

## Topics

### Structures

struct Error

Constants that indicate errors in the WKWebExtension.DataRecord domain.

### Instance Properties

var containedDataTypes: Set&lt;WKWebExtension.DataType>

The set of data types contained in this data record.

var displayName: String

The display name for the web extension to which this data record belongs.

var errors: [any Error]

An array of errors that may have occurred when either calculating or deleting storage.

var totalSizeInBytes: Int

The total size in bytes of all data types contained in this data record.

var uniqueIdentifier: String

Unique identifier for the web extension context to which this data record belongs.

### Instance Methods

func sizeInBytes(ofTypes: Set&lt;WKWebExtension.DataType>) -> Int

Retrieves the size in bytes of the specific data types in this data record.

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

