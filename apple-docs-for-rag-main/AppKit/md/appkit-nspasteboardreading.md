

- AppKit
-  NSPasteboardReading 

Protocol

# NSPasteboardReading

A set of methods that defines the interface for initializing an object from a pasteboard.

macOS

``` source
protocol NSPasteboardReading : NSObjectProtocol
```

## Overview

The Cocoa framework classes NSString, NSAttributedString, NSURL, NSColor, NSSound, NSImage, and NSPasteboardItem implement this protocol. You can make your custom class conform to this protocol so that you can read instances from a pasteboard using the readObjects(forClasses:options:) method of NSPasteboard.

## Topics

### Initializing the Pasteboard

init?(pasteboardPropertyList: Any, ofType: NSPasteboard.PasteboardType)

Initializes an instance with a property list object and a type string.

**Required**

### Reading From the Pasteboard

static func readableTypes(for: NSPasteboard) -> [NSPasteboard.PasteboardType]

Returns an array of uniform type identifier strings of data types the receiver can read from the pasteboard and initialize from.

**Required**

static func readingOptions(forType: NSPasteboard.PasteboardType, pasteboard: NSPasteboard) -> NSPasteboard.ReadingOptions

Returns options for reading data of a specified type from a given pasteboard.

struct ReadingOptions

Options that specify how to interpret data on the pasteboard when initializing pasteboard data.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSColor
- NSFilePromiseReceiver
- NSImage
- NSPasteboardItem
- NSSound
- NSTextStorage

## See Also

### Pasteboard

class NSPasteboard

An object that transfers data to and from the pasteboard server.

class NSPasteboardItem

An item on a pasteboard.

protocol NSPasteboardWriting

A set of methods that defines the interface for retrieving a representation of an object that can be written to a pasteboard.

protocol NSPasteboardItemDataProvider

A set of methods implemented by the data provider of a pasteboard item to provide the data for a particular UTI type.

struct ContentsOptions

Options for preparing the pasteboard.

protocol NSPasteboardTypeOwner

An object that serves as a data provider for data types that use lazy data fulfillment from a pasteboard request.

