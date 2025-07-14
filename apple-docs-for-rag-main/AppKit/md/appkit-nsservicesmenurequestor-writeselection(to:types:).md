

- AppKit
- NSServicesMenuRequestor
-  writeSelection(to:types:) 

Instance Method

# writeSelection(to:types:)

Writes the current selection to the pasteboard.

macOS

``` source
optional func writeSelection(
    to pboard: NSPasteboard,
    types: [NSPasteboard.PasteboardType]
) -> Bool
```

## Parameters 

`pboard`  

The pasteboard to receive your data.

`types`  

An array of `NSString` objects listing the types of data that you should write to the pasteboard. You should write data to the pasteboard for as many of the types as you support.

## Return Value

true if your implementation was able to write one or more types to the pasteboard; otherwise, false.

## Mentioned in 

Supporting Writing Tools via the pasteboard

## Discussion

A writeSelection(to:types:) message is sent to the first responder when the user chooses a command from the Services menu, but only if the receiver didn’t return `nil` to a previous validRequestor(forSendType:returnType:) message.

After your method writes the data to the pasteboard, a remote message is sent to the application that provides the service the user requested. If the service provider supplies return data to replace the selection, the first responder will then receive a readSelection(from:) message.

## See Also

### Related Documentation

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Overridden by subclasses to determine what services are available.

### Working with Pasteboards

func readSelection(from: NSPasteboard) -> Bool

Reads data from the pasteboard and uses it to replace the current selection.

