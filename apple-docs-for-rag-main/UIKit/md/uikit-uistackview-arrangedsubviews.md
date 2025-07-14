

- UIKit
- UIStackView
-  arrangedSubviews 

Instance Property

# arrangedSubviews

The list of views arranged by the stack view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var arrangedSubviews: [UIView] { get }
```

## Discussion

The stack view ensures that the arrangedSubviews array is always a subset of its subviews array. Therefore, whenever the addArrangedSubview(_:) method is called, the stack view adds the view as a subview, if it isn’t already. Whenever an arranged view’s removeFromSuperview() method is called, the stack view removes the view from its arrangedSubviews array.

## See Also

### Related Documentation

func removeFromSuperview()

Unlinks the view from its superview and its window, and removes it from the responder chain.

convenience init(arrangedSubviews: [UIView])

Returns a new stack view object that manages the provided views.

### Managing arranged subviews

func addArrangedSubview(UIView)

Adds a view to the end of the arranged subviews array.

func insertArrangedSubview(UIView, at: Int)

Adds the provided view to the array of arranged subviews at the specified index.

func removeArrangedSubview(UIView)

Removes the provided view from the stack’s array of arranged subviews.

