

- AppKit
- NSStackView
-  insertArrangedSubview(\_:at:) 

Instance Method

# insertArrangedSubview(\_:at:)

Adds the provided view to the array of arranged subviews at the specified index.

macOS 10.11+

``` source
@MainActor
func insertArrangedSubview(
    _ view: NSView,
    at index: Int
)
```

## Parameters 

`view`  

The view to be added to the array of arranged views managed by the stack.

`index`  

The index where the stack inserts the new view in its arrangedSubviews array. This value must not be greater than the number of views currently in this array. If the index is out of bounds, this method throws an internalInconsistencyException exception.

## Discussion

If index is already occupied, the stack view increases the size of the arrangedSubviews array and shifts all of its contents at the index and above to the next higher space in the array. Then the stack view stores the provided view at the index.

The stack view also ensures that the arrangedSubviews array is always a subset of its subviews array. This method automatically adds the provided view as a subview of the stack view, if it is not already. When adding subviews, the stack view appends the view to the end of its subviews array. The index only affects the order of views in the arrangedSubviews array. It does not affect the ordering of views in the subviews array.

## See Also

### Managing the Arranged Subviews

func addArrangedSubview(NSView)

Adds the specified view to the end of the arranged subviews list.

func removeArrangedSubview(NSView)

Removes the provided view from the stack’s array of arranged subviews.

var arrangedSubviews: [NSView]

The array of views arranged by the stack view.

