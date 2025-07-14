

- Assignables
- AssignedWorkDocumentView
-  padding3D(\_:\_:) 

Instance Method

# padding3D(\_:\_:)

Pads this view using the edge insets you specify.

AssignablesSwiftUIvisionOS 1.0+

``` source
nonisolated
func padding3D(
    _ edges: Edge3D.Set = .all,
    _ length: CGFloat? = nil
) -> some View
```

## Parameters 

`edges`  

The set of edges along which to inset this view.

`length`  

The amount to inset this view on each edge. If `nil`, the amount is the system default amount.

## Return Value

A view that pads this view using edge the insets you specify.

