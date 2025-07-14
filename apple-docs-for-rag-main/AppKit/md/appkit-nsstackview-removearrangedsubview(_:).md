

- AppKit
- NSStackView
-  removeArrangedSubview(\_:) 

Instance Method

# removeArrangedSubview(\_:)

Removes the provided view from the stack’s array of arranged subviews.

macOS 10.11+

``` source
@MainActor
func removeArrangedSubview(_ view: NSView)
```

## Parameters 

`view`  

The view to be removed from the array of views arranged by the stack.

## Discussion

This method removes the provided view from the stack’s arrangedSubviews array. After calling this method, the stack view no longer manages the view’s position and size. However, this method does not remove the provided view from the stack’s subviews array; therefore, the view still appears in the view hierarchy.

To prevent the view from appearing on screen after calling this method, explicitly call the view’s removeFromSuperview() method, or set its isHidden property to true.

## See Also

### Managing the Arranged Subviews

func addArrangedSubview(NSView)

Adds the specified view to the end of the arranged subviews list.

func insertArrangedSubview(NSView, at: Int)

Adds the provided view to the array of arranged subviews at the specified index.

var arrangedSubviews: [NSView]

The array of views arranged by the stack view.

