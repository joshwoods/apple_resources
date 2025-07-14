

- AppKit
- NSTokenFieldCellDelegate
-  tokenFieldCell(\_:readFrom:) 

Instance Method

# tokenFieldCell(\_:readFrom:)

Allows the delegate to return an array of objects representing the data read from `pboard`.

macOS

``` source
@MainActor
optional func tokenFieldCell(
    _ tokenFieldCell: NSTokenFieldCell,
    readFrom pboard: NSPasteboard
) -> [Any]?
```

## Parameters 

`tokenFieldCell`  

The token field cell that sent the message.

`pboard`  

The pasteboard from which to read the represented objects.

## Return Value

An array of represented objects created from the pasteboard data.

## See Also

### Reading To and Writing From the Pasteboard

func tokenFieldCell(NSTokenFieldCell, writeRepresentedObjects: [Any], to: NSPasteboard) -> Bool

Allows the delegate the opportunity to write custom pasteboard types to the pasteboard for the represented objects in `objects`.

