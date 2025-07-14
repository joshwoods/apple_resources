

- SwiftUI
- View
-  padding3D(\_:\_:) 

Instance Method

# padding3D(\_:\_:)

Pads this view using the edge insets you specify.

visionOS 1.0+

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

## See Also

### Adding padding around a view

func padding(_:)

Adds a different padding amount to each edge of this view.

func padding(Edge.Set, CGFloat?) -> some View

Adds an equal padding amount to specific edges of this view.

func padding3D(_:)

Pads this view using the edge insets you specify.

func scenePadding(Edge.Set) -> some View

Adds padding to the specified edges of this view using an amount that’s appropriate for the current scene.

func scenePadding(ScenePadding, edges: Edge.Set) -> some View

Adds a specified kind of padding to the specified edges of this view using an amount that’s appropriate for the current scene.

struct ScenePadding

The padding used to space a view from its containing scene.

