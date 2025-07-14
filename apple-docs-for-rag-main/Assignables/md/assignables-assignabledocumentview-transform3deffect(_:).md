

- Assignables
- AssignableDocumentView
-  transform3DEffect(\_:) 

Instance Method

# transform3DEffect(\_:)

Applies a 3D transformation to the receiver.

AssignablesSwiftUIvisionOS 1.0+

``` source
nonisolated
func transform3DEffect(_ transform: AffineTransform3D) -> some View
```

## Parameters 

`transform`  

The 3D transformation to apply to the view, interpreting it as a 3D plane in space.

## Return Value

A view that renders transformed according to the provided `transform`

