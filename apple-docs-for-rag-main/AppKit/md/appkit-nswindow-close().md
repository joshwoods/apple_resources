

- AppKit
- NSWindow
-  close() 

Instance Method

# close()

Removes the window from the screen.

macOS

``` source
@MainActor
func close()
```

## Discussion

If the window is set to be released when closed, a `release` message is sent to the object after the current event is completed. For an `NSWindow` object, the default is to be released on closing, while for an NSPanel object, the default is not to be released. You can use the isReleasedWhenClosed property to change the default behavior.

A window doesn’t have to be visible to receive the close message. For example, when the application terminates, it sends the close message to all windows in its window list, even those that are not currently visible.

The close method posts a willCloseNotification notification to the default notification center.

The close method differs in two important ways from the performClose(_:) method:

- It does not attempt to send a windowShouldClose(_:) message to the window or its delegate.

- It does not simulate the user clicking the close button by momentarily highlighting the button.

Use performClose(_:) if you need these features.

## See Also

### Related Documentation

func orderOut(Any?)

Removes the window from the screen list, which hides the window.

### Closing Windows

func performClose(Any?)

Simulates the user clicking the close button by momentarily highlighting the button and then closing the window.

var isReleasedWhenClosed: Bool

A Boolean value that indicates whether the window is released when it receives the `close` message.

