

- AppKit
- NSPasteboard
-  index(of:) 

Instance Method

# index(of:)

Returns the index of the specified pasteboard item.

macOS 10.6+

``` source
func index(of pasteboardItem: NSPasteboardItem) -> Int
```

## Parameters 

`pasteboardItem`  

A pasteboard item.

## Return Value

The index of the specified pasteboard item. If `pasteboardItem` has not been added to any pasteboard, or is owned by another pasteboard, returns `NSNotFound`.

## Discussion

An item’s index in the pasteboard is useful for a pasteboard item data provider that has promised data for multiple items, to be able to easily match the pasteboard item to an array of source data from which to derive the promised data.

## See Also

### Reading Data

func readObjects(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> [Any]?

Reads from the receiver objects that best match the specified array of classes.

struct ReadingOptionKey

Options for reading pasteboard data.

struct ReadingOptions

Options that specify how to interpret data on the pasteboard when initializing pasteboard data.

var pasteboardItems: [NSPasteboardItem]?

An array that contains all the items held by the pasteboard.

func data(forType: NSPasteboard.PasteboardType) -> Data?

Returns the data for the specified type from the first item in the receiver that contains the type.

func propertyList(forType: NSPasteboard.PasteboardType) -> Any?

Returns the property list for the specified type from the first item in the receiver that contains the type.

func string(forType: NSPasteboard.PasteboardType) -> String?

Returns a concatenation of the strings for the specified type from all the items in the receiver that contain the type.

