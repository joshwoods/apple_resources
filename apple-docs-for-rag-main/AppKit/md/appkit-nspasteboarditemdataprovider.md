

- AppKit
-  NSPasteboardItemDataProvider 

Protocol

# NSPasteboardItemDataProvider

A set of methods implemented by the data provider of a pasteboard item to provide the data for a particular UTI type.

macOS

``` source
protocol NSPasteboardItemDataProvider : NSObjectProtocol
```

## Overview

You can specify an object as a pasteboard data provider for a pasteboard item using NSPasteboardItem’s setDataProvider(_:forTypes:) method. The data provider must implement this protocol to provide data upon request.

## Topics

### Providing Data

func pasteboard(NSPasteboard?, item: NSPasteboardItem, provideDataForType: NSPasteboard.PasteboardType)

Asks the receiver to provide data for a specified type to a given pasteboard.

**Required**

func pasteboardFinishedWithDataProvider(NSPasteboard)

Informs the receiver that the pasteboard no longer needs the data provider for any of its pasteboard items.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Pasteboard

class NSPasteboard

An object that transfers data to and from the pasteboard server.

class NSPasteboardItem

An item on a pasteboard.

protocol NSPasteboardReading

A set of methods that defines the interface for initializing an object from a pasteboard.

protocol NSPasteboardWriting

A set of methods that defines the interface for retrieving a representation of an object that can be written to a pasteboard.

struct ContentsOptions

Options for preparing the pasteboard.

protocol NSPasteboardTypeOwner

An object that serves as a data provider for data types that use lazy data fulfillment from a pasteboard request.

