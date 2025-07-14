

- SwiftUI
- WindowLayoutRoot
-  sizeThatFits(\_:) 

Instance Method

# sizeThatFits(\_:)

Asks the window’s content for its size.

macOS 15.0+visionOS 2.0+

``` source
func sizeThatFits(_ proposal: ProposedViewSize) -> CGSize
```

## Parameters 

`proposal`  

A proposed size for the subview. In SwiftUI, views choose their own size, but can take a size proposal from their parent view into account when doing so.

## Return Value

The size that the content chooses for itself, given the proposal from its container view.

