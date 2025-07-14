

- AppKit
-  NSPasteboardTypeOwner 

Protocol

# NSPasteboardTypeOwner

An object that serves as a data provider for data types that use lazy data fulfillment from a pasteboard request.

macOS

``` source
protocol NSPasteboardTypeOwner : NSObjectProtocol
```

## Topics

### Fulfilling lazy data requests

func pasteboard(NSPasteboard, provideDataForType: NSPasteboard.PasteboardType)

Requests that the object provide data for the data type to the pasteboard.

**Required**

### Changing pasteboard ownership

func pasteboardChangedOwner(NSPasteboard)

Notifies the object that the pasteboard’s owner changed.

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

protocol NSPasteboardItemDataProvider

A set of methods implemented by the data provider of a pasteboard item to provide the data for a particular UTI type.

struct ContentsOptions

Options for preparing the pasteboard.

