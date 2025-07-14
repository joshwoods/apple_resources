

- AppKit
- NSWindowDelegate
-  windowShouldClose(\_:) 

Instance Method

# windowShouldClose(\_:)

Tells the delegate that the user has attempted to close a window or the window has received a performClose(_:) message.

macOS

``` source
@MainActor
optional func windowShouldClose(_ sender: NSWindow) -> Bool
```

## Parameters 

`sender`  

The window being closed.

## Return Value

true to allow `sender` to be closed; otherwise, false.

## Discussion

This method may not always be called during window closing. Specifically, this method is not called when a user quits an application.

## See Also

### Closing Windows

func windowWillClose(Notification)

Tells the delegate that the window is about to close.

