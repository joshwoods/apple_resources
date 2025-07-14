

- AppKit
- NSVisualEffectView
-  viewDidMoveToWindow() 

Instance Method

# viewDidMoveToWindow()

Notifies the view that it moved to a new window.

macOS 10.10+

``` source
@MainActor
func viewDidMoveToWindow()
```

## Discussion

When subclassing, you can override this method and use it to perform any tasks associated with the change. You must call `super` at some point during your implementation.

## See Also

### Handling Moves to a Different Window

func viewWillMove(toWindow: NSWindow?)

Notifies the view immediately before it moves to a new window (which may be `nil`).

