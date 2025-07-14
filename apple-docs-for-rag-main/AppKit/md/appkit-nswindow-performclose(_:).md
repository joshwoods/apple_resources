

- AppKit
- NSWindow
-  performClose(\_:) 

Instance Method

# performClose(\_:)

Simulates the user clicking the close button by momentarily highlighting the button and then closing the window.

macOS

``` source
@MainActor
func performClose(_ sender: Any?)
```

## Parameters 

`sender`  

The message’s sender.

## Discussion

If the window’s delegate or the window itself implements windowShouldClose(_:), the window sends that message with the window as the argument. The window sends only one such message; if both the delegate and the window implement the method, the delegate receives the message. If the windowShouldClose(_:) method returns false, the window doesn’t close. If neither the window nor the delegate implement windowShouldClose(_:), or it returns true, this method invokes close() to close the window.

If the window doesn’t have a close button or can’t close (for example, if the delegate replies false to a windowShouldClose(_:) message), the system emits the alert sound.

## See Also

### Related Documentation

var styleMask: NSWindow.StyleMask

Flags that describe the window’s current style, such as if it’s resizable or in full-screen mode.

func performMiniaturize(Any?)

Simulates the user clicking the minimize button by momentarily highlighting the button, then minimizing the window.

### Closing Windows

func close()

Removes the window from the screen.

var isReleasedWhenClosed: Bool

A Boolean value that indicates whether the window is released when it receives the `close` message.

