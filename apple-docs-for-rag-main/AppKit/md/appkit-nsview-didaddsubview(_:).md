

- AppKit
- NSView
-  didAddSubview(\_:) 

Instance Method

# didAddSubview(\_:)

Overridden by subclasses to perform additional actions when subviews are added to the view.

macOS

``` source
@MainActor
func didAddSubview(_ subview: NSView)
```

## Parameters 

`subview`  

The view that was added as a subview.

## Discussion

This method is invoked by addSubview(_:).

## See Also

### Responding to View-Related Notifications

func viewDidMoveToSuperview()

Informs the view that its superview has changed (possibly to `nil`).

func viewDidMoveToWindow()

Informs the view that it has been added to a new view hierarchy.

func viewWillMove(toSuperview: NSView?)

Informs the view that its superview is about to change to the specified superview (which may be `nil`).

func viewWillMove(toWindow: NSWindow?)

Informs the view that it’s being added to the view hierarchy of the specified window object (which may be `nil`).

func willRemoveSubview(NSView)

Overridden by subclasses to perform additional actions before subviews are removed from the view.

