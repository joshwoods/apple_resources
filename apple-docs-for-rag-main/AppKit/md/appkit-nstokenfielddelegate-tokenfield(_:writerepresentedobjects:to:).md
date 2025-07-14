

- AppKit
- NSTokenFieldDelegate
-  tokenField(\_:writeRepresentedObjects:to:) 

Instance Method

# tokenField(\_:writeRepresentedObjects:to:)

Sent so the delegate can write represented objects to the pasteboard corresponding to a given array of display strings.

macOS

``` source
@MainActor
optional func tokenField(
    _ tokenField: NSTokenField,
    writeRepresentedObjects objects: [Any],
    to pboard: NSPasteboard
) -> Bool
```

## Parameters 

`tokenField`  

The token field that sent the message.

`objects`  

An array of represented objects associated with the token field.

`pboard`  

The pasteboard to which to write the represented objects.

## Return Value

true if the delegate writes the represented objects to the pasteboard, false otherwise. If false, the token field writes the display strings to the NSStringPboardType pasteboard.

## See Also

### Reading To and Writing From the Pasteboard

func tokenField(NSTokenField, readFrom: NSPasteboard) -> [Any]?

Allows the delegate to return an array of objects representing the data read from the specified pasteboard.

