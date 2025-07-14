

- UIKit
- UIStackView
-  removeArrangedSubview(\_:) 

Instance Method

# removeArrangedSubview(\_:)

Removes the provided view from the stack’s array of arranged subviews.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func removeArrangedSubview(_ view: UIView)
```

## Parameters 

`view`  

The view to be removed from the array of views arranged by the stack.

## Discussion

This method removes the provided view from the stack’s arrangedSubviews array. The stack view no longer manages the view’s position and size. However, this method doesn’t remove the provided view from the stack’s subviews array; therefore, the view is still displayed as part of the view hierarchy.

To prevent the view from appearing on screen after calling the stack’s removeArrangedSubview(_:) method, explicitly remove the view from the subviews array by calling the view’s removeFromSuperview() method, or set the view’s isHidden property to true.

## See Also

### Related Documentation

func removeFromSuperview()

Unlinks the view from its superview and its window, and removes it from the responder chain.

convenience init(arrangedSubviews: [UIView])

Returns a new stack view object that manages the provided views.

### Managing arranged subviews

func addArrangedSubview(UIView)

Adds a view to the end of the arranged subviews array.

var arrangedSubviews: [UIView]

The list of views arranged by the stack view.

func insertArrangedSubview(UIView, at: Int)

Adds the provided view to the array of arranged subviews at the specified index.

