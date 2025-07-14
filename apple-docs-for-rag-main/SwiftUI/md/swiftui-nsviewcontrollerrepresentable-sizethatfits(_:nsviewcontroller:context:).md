

- SwiftUI
- NSViewControllerRepresentable
-  sizeThatFits(\_:nsViewController:context:) 

Instance Method

# sizeThatFits(\_:nsViewController:context:)

Given a proposed size, returns the preferred size of the composite view.

macOS 13.0+

``` source
@MainActor @preconcurrency
func sizeThatFits(
    _ proposal: ProposedViewSize,
    nsViewController: Self.NSViewControllerType,
    context: Self.Context
) -> CGSize?
```

**Required** Default implementation provided.

## Parameters 

`proposal`  

The proposed size for the view controller.

`nsViewController`  

Your custom view controller object.

`context`  

A context structure containing information about the current state of the system.

## Return Value

The composite size of the represented view controller. Returning a value of `nil` indicates that the system should use the default sizing algorithm.

## Discussion

This method may be called more than once with different proposed sizes during the same layout pass. SwiftUI views choose their own size, so one of the values returned from this function will always be used as the actual size of the composite view.

## Default Implementations

### NSViewControllerRepresentable Implementations

func sizeThatFits(ProposedViewSize, nsViewController: Self.NSViewControllerType, context: Self.Context) -> CGSize?

Given a proposed size, returns the preferred size of the composite view.

