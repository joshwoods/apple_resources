

- AppKit
- NSVisualEffectView
-  viewWillMove(toWindow:) 

Instance Method

# viewWillMove(toWindow:)

Notifies the view immediately before it moves to a new window (which may be `nil`).

macOS 10.10+

``` source
@MainActor
func viewWillMove(toWindow newWindow: NSWindow?)
```

## Parameters 

`newWindow`  

The window object that will be at the root of the view’s new view hierarchy. If the view is being removed from a window and there isn’t a new window, this parameter is `nil`.

## Discussion

When subclassing, you can override this method and use it to perform any tasks associated with the change. You must call `super` at some point during your implementation.

## See Also

### Handling Moves to a Different Window

func viewDidMoveToWindow()

Notifies the view that it moved to a new window.

