

- UIKit
- UIStackView
-  init(arrangedSubviews:) 

Initializer

# init(arrangedSubviews:)

Returns a new stack view object that manages the provided views.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
convenience init(arrangedSubviews views: [UIView])
```

## Parameters 

`views`  

The views to be arranged by the stack view.

## Return Value

A new stack view object. This stack view contains and lays out the provided views in a single stack. You can modify the orientation or appearance of this stack, using the stack view’s properties.

## Discussion

The stack view adds all the arranged views to its arrangedSubviews array. It also adds these views as subviews. If any view contained in the `arrangedSubviews` array receives a removeFromSuperview() method call, the stack view also removes it from the `arrangedSubviews`.

## See Also

### Related Documentation

func insertArrangedSubview(UIView, at: Int)

Adds the provided view to the array of arranged subviews at the specified index.

func removeFromSuperview()

Unlinks the view from its superview and its window, and removes it from the responder chain.

var arrangedSubviews: [UIView]

The list of views arranged by the stack view.

func addArrangedSubview(UIView)

Adds a view to the end of the arranged subviews array.

func removeArrangedSubview(UIView)

Removes the provided view from the stack’s array of arranged subviews.

### Initializing a stack view

init(frame: CGRect)

Creates a stack view with the specified frame.

init(coder: NSCoder)

Creates a stack view from data in an unarchiver.

