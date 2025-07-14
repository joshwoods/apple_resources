

- AppKit
- NSPasteboardReading
-  readableTypes(for:) 

Type Method

# readableTypes(for:)

Returns an array of uniform type identifier strings of data types the receiver can read from the pasteboard and initialize from.

macOS

``` source
static func readableTypes(for pasteboard: NSPasteboard) -> [NSPasteboard.PasteboardType]
```

**Required**

## Parameters 

`pasteboard`  

A pasteboard. You can use the pasteboard argument to provide different types based on the pasteboard name, if you need to.

## Return Value

An array of uniform type identifier strings of data types instances that the receiver can read from the pasteboard and initialize from.

## Discussion

By default, the system provides the data for a type to init(pasteboardPropertyList:ofType:) as an instance of `NSData`. If you implement readingOptions(forType:pasteboard:) and specify a different option, the system converts the `NSData` object for a type to an `NSString` object or any other property list object.

### Special Considerations

Don’t perform other pasteboard operations in the method implementation.

## See Also

### Reading From the Pasteboard

static func readingOptions(forType: NSPasteboard.PasteboardType, pasteboard: NSPasteboard) -> NSPasteboard.ReadingOptions

Returns options for reading data of a specified type from a given pasteboard.

struct ReadingOptions

Options that specify how to interpret data on the pasteboard when initializing pasteboard data.

