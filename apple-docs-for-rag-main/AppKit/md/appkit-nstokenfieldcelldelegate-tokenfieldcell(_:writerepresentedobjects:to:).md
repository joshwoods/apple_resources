

- AppKit
- NSTokenFieldCellDelegate
-  tokenFieldCell(\_:writeRepresentedObjects:to:) 

Instance Method

# tokenFieldCell(\_:writeRepresentedObjects:to:)

Allows the delegate the opportunity to write custom pasteboard types to the pasteboard for the represented objects in `objects`.

macOS

``` source
@MainActor
optional func tokenFieldCell(
    _ tokenFieldCell: NSTokenFieldCell,
    writeRepresentedObjects objects: [Any],
    to pboard: NSPasteboard
) -> Bool
```

## Parameters 

`tokenFieldCell`  

The token field cell that sent the message.

`objects`  

An array of represented objects associated with the token field cell.

`pboard`  

The pasteboard to which to write the represented objects.

## Return Value

true if the delegate writes the represented objects to the pasteboard, false otherwise. If false, the token field writes the display strings to the NSStringPboardType pasteboard.

## See Also

### Reading To and Writing From the Pasteboard

func tokenFieldCell(NSTokenFieldCell, readFrom: NSPasteboard) -> [Any]?

Allows the delegate to return an array of objects representing the data read from `pboard`.

