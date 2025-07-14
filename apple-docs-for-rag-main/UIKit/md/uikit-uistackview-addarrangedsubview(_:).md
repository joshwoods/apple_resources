

- UIKit
- UIStackView
-  addArrangedSubview(\_:) 

Instance Method

# addArrangedSubview(\_:)

Adds a view to the end of the arranged subviews array.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func addArrangedSubview(_ view: UIView)
```

## Parameters 

`view`  

The view to add to the array of views arranged by the stack.

## Discussion

The stack view ensures that the arrangedSubviews array is always a subset of its subviews array. This method automatically adds the provided view as a subview of the stack view, if it isn’t already. If the view is already a subview, this operation doesn’t alter the subview ordering.

## See Also

### Related Documentation

func removeFromSuperview()

Unlinks the view from its superview and its window, and removes it from the responder chain.

convenience init(arrangedSubviews: [UIView])

Returns a new stack view object that manages the provided views.

### Managing arranged subviews

var arrangedSubviews: [UIView]

The list of views arranged by the stack view.

func insertArrangedSubview(UIView, at: Int)

Adds the provided view to the array of arranged subviews at the specified index.

func removeArrangedSubview(UIView)

Removes the provided view from the stack’s array of arranged subviews.

