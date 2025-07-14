

- AppKit
- NSView
-  viewWillMove(toSuperview:) 

Instance Method

# viewWillMove(toSuperview:)

Informs the view that its superview is about to change to the specified superview (which may be `nil`).

macOS

``` source
@MainActor
func viewWillMove(toSuperview newSuperview: NSView?)
```

## Parameters 

`newSuperview`  

A view object that will be the new superview of the view.

## Discussion

Subclasses can override this method to perform whatever actions are necessary.

## See Also

### Responding to View-Related Notifications

func didAddSubview(NSView)

Overridden by subclasses to perform additional actions when subviews are added to the view.

func viewDidMoveToSuperview()

Informs the view that its superview has changed (possibly to `nil`).

func viewDidMoveToWindow()

Informs the view that it has been added to a new view hierarchy.

func viewWillMove(toWindow: NSWindow?)

Informs the view that it’s being added to the view hierarchy of the specified window object (which may be `nil`).

func willRemoveSubview(NSView)

Overridden by subclasses to perform additional actions before subviews are removed from the view.

