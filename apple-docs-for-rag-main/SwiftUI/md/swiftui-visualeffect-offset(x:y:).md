

- SwiftUI
- VisualEffect
-  offset(x:y:) 

Instance Method

# offset(x:y:)

Offsets the view by the specified horizontal and vertical distances.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func offset(
    x: CGFloat = 0,
    y: CGFloat = 0
) -> some VisualEffect
```

## Parameters 

`x`  

The horizontal distance to offset the view.

`y`  

The vertical distance to offset the view.

## Return Value

An effect that offsets the view by `x` and `y`.

## See Also

### Translating

func offset(CGSize) -> some VisualEffect

Offsets the view by the horizontal and vertical amount specified in the offset parameter.

func offset(z: CGFloat) -> some VisualEffect

Brings a view forward in Z by the provided distance in points.

