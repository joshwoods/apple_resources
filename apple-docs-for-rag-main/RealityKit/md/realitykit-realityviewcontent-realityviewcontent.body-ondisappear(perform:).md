

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  onDisappear(perform:) 

Instance Method

# onDisappear(perform:)

Adds an action to perform after this view disappears.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func onDisappear(perform action: (() -> Void)? = nil) -> some View
```

## Parameters 

`action`  

The action to perform. If `action` is `nil`, the call has no effect.

## Return Value

A view that triggers `action` after it disappears.

## Discussion

The exact moment that SwiftUI calls this method depends on the specific view type that you apply it to, but the `action` closure doesn’t execute until the view disappears from the interface.

