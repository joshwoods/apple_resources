

- AppKit
- NSPasteboard
-  NSPasteboard.ReadingOptions 

Structure

# NSPasteboard.ReadingOptions

Options that specify how to interpret data on the pasteboard when initializing pasteboard data.

macOS 10.6+

``` source
struct ReadingOptions
```

## Overview

You can specify only one option. If you don’t specify an option, the system uses the default asData.

## Topics

### Options

static var asData: NSPasteboard.ReadingOptions

An option to read data from the pasteboard as-is and return it as a data object.

static var asString: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and convert it to a string object.

static var asPropertyList: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and unserialize it as a property list.

static var asKeyedArchive: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and use it to initialize the object.

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

### Reading Data

func readObjects(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> [Any]?

Reads from the receiver objects that best match the specified array of classes.

struct ReadingOptionKey

Options for reading pasteboard data.

var pasteboardItems: [NSPasteboardItem]?

An array that contains all the items held by the pasteboard.

func index(of: NSPasteboardItem) -> Int

Returns the index of the specified pasteboard item.

func data(forType: NSPasteboard.PasteboardType) -> Data?

Returns the data for the specified type from the first item in the receiver that contains the type.

func propertyList(forType: NSPasteboard.PasteboardType) -> Any?

Returns the property list for the specified type from the first item in the receiver that contains the type.

func string(forType: NSPasteboard.PasteboardType) -> String?

Returns a concatenation of the strings for the specified type from all the items in the receiver that contain the type.

