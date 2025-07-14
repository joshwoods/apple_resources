

- AppKit
- NSPasteboardReading
-  readingOptions(forType:pasteboard:) 

Type Method

# readingOptions(forType:pasteboard:)

Returns options for reading data of a specified type from a given pasteboard.

macOS 10.6+

``` source
optional static func readingOptions(
    forType type: NSPasteboard.PasteboardType,
    pasteboard: NSPasteboard
) -> NSPasteboard.ReadingOptions
```

## Parameters 

`type`  

A UTI supported by instances of the receiver for reading (one of the types returned by readableTypes(for:)).

`pasteboard`  

A pasteboard.

You can use the pasteboard argument to provide return different based on the pasteboard name, should you need to do so.

## Return Value

Options for reading data of `type` from `pasteboard`. For a list of valid values, see NSPasteboard.ReadingOptions.

## Discussion

Do not perform other pasteboard operations in this method implementation.

## See Also

### Reading From the Pasteboard

static func readableTypes(for: NSPasteboard) -> [NSPasteboard.PasteboardType]

Returns an array of uniform type identifier strings of data types the receiver can read from the pasteboard and initialize from.

**Required**

struct ReadingOptions

Options that specify how to interpret data on the pasteboard when initializing pasteboard data.

