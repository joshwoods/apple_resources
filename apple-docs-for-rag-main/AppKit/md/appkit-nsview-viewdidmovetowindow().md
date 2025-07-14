

- AppKit
- NSView
-  viewDidMoveToWindow() 

Instance Method

# viewDidMoveToWindow()

Informs the view that it has been added to a new view hierarchy.

macOS

``` source
@MainActor
func viewDidMoveToWindow()
```

## Discussion

The default implementation does nothing; subclasses can override this method to perform whatever actions are necessary.

If the view’s window property is `nil`, that result signifies that the view was removed from its window and does not currently reside in any window.

## See Also

### Responding to View-Related Notifications

func didAddSubview(NSView)

Overridden by subclasses to perform additional actions when subviews are added to the view.

func viewDidMoveToSuperview()

Informs the view that its superview has changed (possibly to `nil`).

func viewWillMove(toSuperview: NSView?)

Informs the view that its superview is about to change to the specified superview (which may be `nil`).

func viewWillMove(toWindow: NSWindow?)

Informs the view that it’s being added to the view hierarchy of the specified window object (which may be `nil`).

func willRemoveSubview(NSView)

Overridden by subclasses to perform additional actions before subviews are removed from the view.

