

- AppKit
- NSPasteboard
-  pasteboardItems 

Instance Property

# pasteboardItems

An array that contains all the items held by the pasteboard.

macOS 10.6+

``` source
var pasteboardItems: [NSPasteboardItem]? { get }
```

## Discussion

If an error occurs when retrieving the pasteboard items, the value of this property is `nil`.

## See Also

### Reading Data

func readObjects(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> [Any]?

Reads from the receiver objects that best match the specified array of classes.

struct ReadingOptionKey

Options for reading pasteboard data.

struct ReadingOptions

Options that specify how to interpret data on the pasteboard when initializing pasteboard data.

func index(of: NSPasteboardItem) -> Int

Returns the index of the specified pasteboard item.

func data(forType: NSPasteboard.PasteboardType) -> Data?

Returns the data for the specified type from the first item in the receiver that contains the type.

func propertyList(forType: NSPasteboard.PasteboardType) -> Any?

Returns the property list for the specified type from the first item in the receiver that contains the type.

func string(forType: NSPasteboard.PasteboardType) -> String?

Returns a concatenation of the strings for the specified type from all the items in the receiver that contain the type.

