

- ManagedAppDistribution
- ManagedContentView
-  onHover(perform:) 

Instance Method

# onHover(perform:)

Adds an action to perform when the user moves the pointer over or away from the view’s frame.

ManagedAppDistributionSwiftUIiOS 13.4+iPadOS 13.4+macOS 10.15+

``` source
nonisolated
func onHover(perform action: @escaping (Bool) -> Void) -> some View
```

## Parameters 

`action`  

The action to perform whenever the pointer enters or exits this view’s frame. If the pointer is in the view’s frame, the `action` closure passes `true` as a parameter; otherwise, `false`.

## Return Value

A view that triggers `action` when the pointer enters or exits this view’s frame.

## Discussion

Calling this method defines a region for detecting pointer movement with the size and position of this view.

