

- AppKit
- NSTokenFieldDelegate
-  tokenField(\_:readFrom:) 

Instance Method

# tokenField(\_:readFrom:)

Allows the delegate to return an array of objects representing the data read from the specified pasteboard.

macOS

``` source
@MainActor
optional func tokenField(
    _ tokenField: NSTokenField,
    readFrom pboard: NSPasteboard
) -> [Any]?
```

## Parameters 

`tokenField`  

The token field that sent the message.

`pboard`  

The pasteboard from which to read the represented objects.

## Return Value

An array of represented objects created from the pasteboard data.

## See Also

### Reading To and Writing From the Pasteboard

func tokenField(NSTokenField, writeRepresentedObjects: [Any], to: NSPasteboard) -> Bool

Sent so the delegate can write represented objects to the pasteboard corresponding to a given array of display strings.

