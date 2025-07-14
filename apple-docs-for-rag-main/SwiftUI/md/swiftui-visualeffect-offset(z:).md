

- SwiftUI
- VisualEffect
-  offset(z:) 

Instance Method

# offset(z:)

Brings a view forward in Z by the provided distance in points.

visionOS 1.0+

``` source
func offset(z: CGFloat) -> some VisualEffect
```

## Return Value

An effect that is extruded forward in Z by `distance`.

## See Also

### Translating

func offset(CGSize) -> some VisualEffect

Offsets the view by the horizontal and vertical amount specified in the offset parameter.

func offset(x: CGFloat, y: CGFloat) -> some VisualEffect

Offsets the view by the specified horizontal and vertical distances.

