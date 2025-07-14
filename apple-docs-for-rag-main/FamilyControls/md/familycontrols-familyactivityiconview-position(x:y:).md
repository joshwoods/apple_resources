

- FamilyControls
- FamilyActivityIconView
-  position(x:y:) 

Instance Method

# position(x:y:)

Positions the center of this view at the specified coordinates in its parent’s coordinate space.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func position(
    x: CGFloat = 0,
    y: CGFloat = 0
) -> some View
```

## Parameters 

`x`  

The x-coordinate at which to place the center of this view.

`y`  

The y-coordinate at which to place the center of this view.

## Return Value

A view that fixes the center of this view at `x` and `y`.

## Discussion

Use the `position(x:y:)` modifier to place the center of a view at a specific coordinate in the parent view using an `x` and `y` offset.

```
Text("Position by passing the x and y coordinates")
    .position(x: 175, y: 100)
    .border(Color.gray)
```

