

- AppKit
- NSStackView
-  addArrangedSubview(\_:) 

Instance Method

# addArrangedSubview(\_:)

Adds the specified view to the end of the arranged subviews list.

macOS 10.11+

``` source
@MainActor
func addArrangedSubview(_ view: NSView)
```

## Parameters 

`view`  

The view to add to the end of the arrangedSubviews array.

## Discussion

The stack view ensures that the arrangedSubviews array is always a subset of its subviews array. This method automatically adds the provided view as a subview of the stack view, if it is not already. If the view is already a subview, this operation does not alter the subview ordering.

## See Also

### Managing the Arranged Subviews

func insertArrangedSubview(NSView, at: Int)

Adds the provided view to the array of arranged subviews at the specified index.

func removeArrangedSubview(NSView)

Removes the provided view from the stack’s array of arranged subviews.

var arrangedSubviews: [NSView]

The array of views arranged by the stack view.

