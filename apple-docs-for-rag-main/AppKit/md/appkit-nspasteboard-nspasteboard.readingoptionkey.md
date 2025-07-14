

- AppKit
- NSPasteboard
-  NSPasteboard.ReadingOptionKey 

Structure

# NSPasteboard.ReadingOptionKey

Options for reading pasteboard data.

macOS

``` source
struct ReadingOptionKey
```

## Discussion

These options can be used for both the readObjects(forClasses:options:) and canReadObject(forClasses:options:) methods, unless otherwise specified. The currently available options allow for customization of how URLS are read from the pasteboard.

## Topics

### Type Properties

static let urlReadingContentsConformToTypes: NSPasteboard.ReadingOptionKey

Option for reading URLs to restrict the results to URLs with contents that conform to any of the provided UTI types.

static let urlReadingFileURLsOnly: NSPasteboard.ReadingOptionKey

Option for reading URLs to restrict the results to file URLs only.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Reading Data

func readObjects(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> [Any]?

Reads from the receiver objects that best match the specified array of classes.

struct ReadingOptions

Options that specify how to interpret data on the pasteboard when initializing pasteboard data.

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

