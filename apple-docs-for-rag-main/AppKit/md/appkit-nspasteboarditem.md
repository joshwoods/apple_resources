

- AppKit
-  NSPasteboardItem 

Class

# NSPasteboardItem

An item on a pasteboard.

macOS 10.6+

``` source
class NSPasteboardItem
```

## Overview

There are three main uses for an NSPasteboardItem object:

- Providing data on the pasteboard.

You can create one or more pasteboard items, set data or data providers for types, and write them to the pasteboard.

- Customizing data already on the pasteboard.

As a delegate or subclass, you can retrieve the pasteboard items currently on the pasteboard, read the existing types and data, and set new data and data providers for types as necessary.

- Retrieving data from the pasteboard.

You can retrieve pasteboard items from the pasteboard and then read the data for types you’re interested in.

A pasteboard item can be associated with a single pasteboard. When you create an item, you can write it to any pasteboard. When you pass an item to a pasteboard in writeObjects(_:), that item becomes bound to the pasteboard it writes to. When you retrieve items from a pasteboard using pasteboardItems or readObjects(forClasses:options:), the returned items are associated with the messaged pasteboard. Passing an item that is already associated with a pasteboard into writeObjects(_:) causes an exception.

Use pasteboard items during a single pasteboard interaction, rather than retaining and reusing them. A pasteboard item is only valid until the owner of the pasteboard changes.

Important

When a pasteboard item’s owner changes, it becomes stale and its methods return an empty array, `nil`, or false.

## Topics

### Getting types

var types: [NSPasteboard.PasteboardType]

An array of uniform type identifier strings of the data types that the receiver supports.

func availableType(from: [NSPasteboard.PasteboardType]) -> NSPasteboard.PasteboardType?

Returns from a given array of types the first type within the pasteboard item, according to the ordering of types.

### Setting the data provider

func setDataProvider(any NSPasteboardItemDataProvider, forTypes: [NSPasteboard.PasteboardType]) -> Bool

Sets the data provider for the specified types.

### Setting values

func setData(Data, forType: NSPasteboard.PasteboardType) -> Bool

Sets the value for a specified type as a data object.

func setString(String, forType: NSPasteboard.PasteboardType) -> Bool

Sets the value for a specified type as a string.

func setPropertyList(Any, forType: NSPasteboard.PasteboardType) -> Bool

Sets the value for a specified type as a property list.

### Getting values

func data(forType: NSPasteboard.PasteboardType) -> Data?

Returns the value for the specified type as a data object.

func string(forType: NSPasteboard.PasteboardType) -> String?

Returns the value for the specified type as a string.

func propertyList(forType: NSPasteboard.PasteboardType) -> Any?

Returns the value for the specified type as a property list.

### Instance Properties

var collaborationMetadata: SWCollaborationMetadata?

A model object you use for conveying data during a collaboration.

### Instance Methods

func detectedMetadata(for: Set&lt;PartialKeyPath&lt;NSPasteboardItem.DetectedMetadata>>) async throws -> NSPasteboardItem.DetectedMetadata

Determines available metadata from the specified metadata types for this pasteboard item, without notifying the user.

func detectedPatterns(for: Set&lt;PartialKeyPath&lt;NSPasteboardItem.DetectedValues>>) async throws -> Set&lt;PartialKeyPath&lt;NSPasteboardItem.DetectedValues>>

Determines whether this pasteboard item matches the specified patterns, without notifying the user.

func detectedValues(for: Set&lt;PartialKeyPath&lt;NSPasteboardItem.DetectedValues>>) async throws -> NSPasteboardItem.DetectedValues

Determines whether this pasteboard item matches the specified patterns, reading the contents if it finds a match.

### Type Aliases

typealias DetectedMetadata

typealias DetectedValues

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
- NSPasteboardReading
- NSPasteboardWriting

## See Also

### Pasteboard

class NSPasteboard

An object that transfers data to and from the pasteboard server.

protocol NSPasteboardReading

A set of methods that defines the interface for initializing an object from a pasteboard.

protocol NSPasteboardWriting

A set of methods that defines the interface for retrieving a representation of an object that can be written to a pasteboard.

protocol NSPasteboardItemDataProvider

A set of methods implemented by the data provider of a pasteboard item to provide the data for a particular UTI type.

struct ContentsOptions

Options for preparing the pasteboard.

protocol NSPasteboardTypeOwner

An object that serves as a data provider for data types that use lazy data fulfillment from a pasteboard request.

