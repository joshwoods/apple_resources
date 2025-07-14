

- AppKit
- NSView
-  viewDidMoveToSuperview() 

Instance Method

# viewDidMoveToSuperview()

Informs the view that its superview has changed (possibly to `nil`).

macOS

``` source
@MainActor
func viewDidMoveToSuperview()
```

## Discussion

The default implementation does nothing; subclasses can override this method to perform whatever actions are necessary.

## See Also

### Responding to View-Related Notifications

func didAddSubview(NSView)

Overridden by subclasses to perform additional actions when subviews are added to the view.

func viewDidMoveToWindow()

Informs the view that it has been added to a new view hierarchy.

func viewWillMove(toSuperview: NSView?)

Informs the view that its superview is about to change to the specified superview (which may be `nil`).

func viewWillMove(toWindow: NSWindow?)

Informs the view that it’s being added to the view hierarchy of the specified window object (which may be `nil`).

func willRemoveSubview(NSView)

Overridden by subclasses to perform additional actions before subviews are removed from the view.

