

- AppKit
- NSPasteboardWriting
-  writableTypes(for:) 

Instance Method

# writableTypes(for:)

Returns an array of UTI strings of data types the receiver can write to a given pasteboard.

macOS

``` source
func writableTypes(for pasteboard: NSPasteboard) -> [NSPasteboard.PasteboardType]
```

**Required**

## Parameters 

`pasteboard`  

A pasteboard.

You can use this argument to provide different options based on the pasteboard name, if you need to.

## Return Value

An array of UTI strings of data types the receiver can write to `pasteboard`.

## Discussion

By default, data for the first returned type is put onto the pasteboard immediately, with the remaining types being promised.

To change the default behavior, implement -writingOptionsForType:pasteboard: and return promised to lazily provide data for types, return no option to provide the data for that type immediately. Use the pasteboard argument to provide different types based on the pasteboard name, if desired. Do not perform other pasteboard operations in the method implementation.

## See Also

### Related Documentation

Drag and Drop Programming Topics

Pasteboard Programming Guide

Services Implementation Guide

### Required Methods

func writingOptions(forType: NSPasteboard.PasteboardType, pasteboard: NSPasteboard) -> NSPasteboard.WritingOptions

Returns options for writing data of a specified type to a given pasteboard.

struct WritingOptions

Type to specify options for writing to a pasteboard.

