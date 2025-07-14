

- AppKit
- NSView
-  viewWillMove(toWindow:) 

Instance Method

# viewWillMove(toWindow:)

Informs the view that it’s being added to the view hierarchy of the specified window object (which may be `nil`).

macOS

``` source
@MainActor
func viewWillMove(toWindow newWindow: NSWindow?)
```

## Parameters 

`newWindow`  

The window object that will be at the root of the view’s new view hierarchy. If the view is being removed from a window and there is no new window, this parameter is `nil`.

## Discussion

AppKit calls this method when the window of a view changes. It also calls it in cases where a view stays in the same window but its position in its view hierarchy changes. The view that moved also calls this method on all of its subviews, giving each of them a chance to respond to the change.

Subclasses can override this method to perform whatever actions are necessary. For example, when a window is deallocated, you can use this method to remove notification observers and bindings associated with the view.

When a window is deallocated, AppKit calls this method for each view in the window, passing `nil` for the `newWindow` parameter. AppKit does not necessarily call this method when closing a window, though. Closing a window usually just hides the window. Closed windows are deallocated only if their isReleasedWhenClosed method returns true.

## See Also

### Responding to View-Related Notifications

func didAddSubview(NSView)

Overridden by subclasses to perform additional actions when subviews are added to the view.

func viewDidMoveToSuperview()

Informs the view that its superview has changed (possibly to `nil`).

func viewDidMoveToWindow()

Informs the view that it has been added to a new view hierarchy.

func viewWillMove(toSuperview: NSView?)

Informs the view that its superview is about to change to the specified superview (which may be `nil`).

func willRemoveSubview(NSView)

Overridden by subclasses to perform additional actions before subviews are removed from the view.

