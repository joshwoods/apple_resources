

- AppKit
- NSPasteboard
-  NSPasteboard.ContentsOptions 

Structure

# NSPasteboard.ContentsOptions

Options for preparing the pasteboard.

macOS 10.12+

``` source
struct ContentsOptions
```

## Topics

### Options

static var currentHostOnly: NSPasteboard.ContentsOptions

The pasteboard contents are available only on the current device, and not on any other devices.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

protocol NSPasteboardTypeOwner

An object that serves as a data provider for data types that use lazy data fulfillment from a pasteboard request.

