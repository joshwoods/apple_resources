

- AppKit
- NSWindow
-  isReleasedWhenClosed 

Instance Property

# isReleasedWhenClosed

A Boolean value that indicates whether the window is released when it receives the `close` message.

macOS

``` source
@MainActor
var isReleasedWhenClosed: Bool { get set }
```

## Discussion

The value of this property is true if the window is automatically released after being closed; false if it’s simply removed from the screen.

The default for `NSWindow` is true; the default for `NSPanel` is false. Release when closed, however, is ignored for windows owned by window controllers. Another strategy for releasing an `NSWindow` object is to have its delegate autorelease it on receiving a windowShouldClose(_:) message.

## See Also

### Closing Windows

func performClose(Any?)

Simulates the user clicking the close button by momentarily highlighting the button and then closing the window.

func close()

Removes the window from the screen.

