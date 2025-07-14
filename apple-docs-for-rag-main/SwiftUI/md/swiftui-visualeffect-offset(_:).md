

- SwiftUI
- VisualEffect
-  offset(\_:) 

Instance Method

# offset(\_:)

Offsets the view by the horizontal and vertical amount specified in the offset parameter.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func offset(_ offset: CGSize) -> some VisualEffect
```

## Parameters 

`offset`  

The distance to offset the view.

## Return Value

An effect that offsets the view by `offset`.

## See Also

### Translating

func offset(x: CGFloat, y: CGFloat) -> some VisualEffect

Offsets the view by the specified horizontal and vertical distances.

func offset(z: CGFloat) -> some VisualEffect

Brings a view forward in Z by the provided distance in points.

