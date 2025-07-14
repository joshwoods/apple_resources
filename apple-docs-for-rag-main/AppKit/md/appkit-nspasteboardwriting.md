

- AppKit
-  NSPasteboardWriting 

Protocol

# NSPasteboardWriting

A set of methods that defines the interface for retrieving a representation of an object that can be written to a pasteboard.

macOS

``` source
protocol NSPasteboardWriting : NSObjectProtocol
```

## Overview

The Cocoa framework classes NSString, NSAttributedString, NSURL, NSColor, NSSound, NSImage, and NSPasteboardItem implement this protocol. You can make your custom class conform to this protocol so that you can write instances of the class to a pasteboard using the writeObjects(_:) method of NSPasteboard.

## Topics

### Required Methods

func writableTypes(for: NSPasteboard) -> [NSPasteboard.PasteboardType]

Returns an array of UTI strings of data types the receiver can write to a given pasteboard.

**Required**

func writingOptions(forType: NSPasteboard.PasteboardType, pasteboard: NSPasteboard) -> NSPasteboard.WritingOptions

Returns options for writing data of a specified type to a given pasteboard.

struct WritingOptions

Type to specify options for writing to a pasteboard.

### Property List for Type

func pasteboardPropertyList(forType: NSPasteboard.PasteboardType) -> Any?

Returns a property list object to represent the receiver on a pasteboard as an object of a specified type.

**Required**

### Constants

Pasteboard Writing Options

Constant to specify options for writing to a pasteboard, used by writingOptions(forType:pasteboard:).

struct WritingOptions

Type to specify options for writing to a pasteboard.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSColor
- NSFilePromiseProvider
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

protocol NSPasteboardReading

A set of methods that defines the interface for initializing an object from a pasteboard.

protocol NSPasteboardItemDataProvider

A set of methods implemented by the data provider of a pasteboard item to provide the data for a particular UTI type.

struct ContentsOptions

Options for preparing the pasteboard.

protocol NSPasteboardTypeOwner

An object that serves as a data provider for data types that use lazy data fulfillment from a pasteboard request.

