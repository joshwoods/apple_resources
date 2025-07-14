

- AppKit
- NSWindowDelegate
-  windowDidEndSheet(\_:) 

Instance Method

# windowDidEndSheet(\_:)

Tells the delegate that the window has closed a sheet.

macOS 10.10+

``` source
@MainActor
optional func windowDidEndSheet(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didEndSheetNotification.

## Discussion

You can retrieve the window object in question by sending object to `notification`.

## See Also

### Managing Sheets

func window(NSWindow, willPositionSheet: NSWindow, using: NSRect) -> NSRect

Tells the delegate that the window is about to show a sheet at the specified location, giving it the opportunity to return a custom location for the attachment of the sheet to the window.

func windowWillBeginSheet(Notification)

Notifies the delegate that the window is about to open a sheet.

