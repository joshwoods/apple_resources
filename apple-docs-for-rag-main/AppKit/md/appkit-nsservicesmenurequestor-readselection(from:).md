

- AppKit
- NSServicesMenuRequestor
-  readSelection(from:) 

Instance Method

# readSelection(from:)

Reads data from the pasteboard and uses it to replace the current selection.

macOS

``` source
optional func readSelection(from pboard: NSPasteboard) -> Bool
```

## Parameters 

`pboard`  

The pasteboard containing the data to read.

## Return Value

true if your implementation was able to read the pasteboard data successfully; otherwise, false.

## Mentioned in 

Supporting Writing Tools via the pasteboard

Supporting Continuity Camera in Your Mac App

## Discussion

You implement this method to replace your application’s current selection (that is, the text or objects that are currently selected) with the data on the pasteboard. The data would have been placed in the pasteboard by another application in response to a remote message from the Services menu. A readSelection(from:) message is sent to the same object that previously received a writeSelection(to:types:) message.

## See Also

### Related Documentation

Services Implementation Guide

### Working with Pasteboards

func writeSelection(to: NSPasteboard, types: [NSPasteboard.PasteboardType]) -> Bool

Writes the current selection to the pasteboard.

