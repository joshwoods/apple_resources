

- AppKit
- NSPasteboardWriting
-  writingOptions(forType:pasteboard:) 

Instance Method

# writingOptions(forType:pasteboard:)

Returns options for writing data of a specified type to a given pasteboard.

macOS 10.6+

``` source
optional func writingOptions(
    forType type: NSPasteboard.PasteboardType,
    pasteboard: NSPasteboard
) -> NSPasteboard.WritingOptions
```

## Parameters 

`type`  

One of the types the receiver supports for writing (one of the UTIs returned by its implementation of writableTypes(for:)).

`pasteboard`  

A pasteboard.

You can use this argument to provide different options based on the pasteboard name, if you need to.

## Return Value

Options for writing data of type type to `pasteboard`. Return `0` for no options, or a value given in Pasteboard Writing Options.

## Discussion

Do not perform other pasteboard operations in the method implementation.

## See Also

### Required Methods

func writableTypes(for: NSPasteboard) -> [NSPasteboard.PasteboardType]

Returns an array of UTI strings of data types the receiver can write to a given pasteboard.

**Required**

struct WritingOptions

Type to specify options for writing to a pasteboard.

