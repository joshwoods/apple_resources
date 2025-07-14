

- RealityKit
- RealityViewAttachmentBuilderContent
-  handPointerBehavior(\_:) 

Instance Method

# handPointerBehavior(\_:)

Sets the behavior of the hand pointer while the user is interacting with the view.

RealityKitSwiftUIvisionOS 2.0+

``` source
nonisolated
func handPointerBehavior(_ behavior: HandPointerBehavior?) -> some View
```

## Parameters 

`behavior`  

The behavior to apply to the hand pointer. If `nil`, the hand pointer behavior will be inherited from the view’s ancestors.

## Return Value

A view that applies the given behavior to the hand pointer.

