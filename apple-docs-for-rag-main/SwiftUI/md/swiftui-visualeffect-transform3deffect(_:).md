

- SwiftUI
- VisualEffect
-  transform3DEffect(\_:) 

Instance Method

# transform3DEffect(\_:)

Applies a 3D transformation to the receiver.

visionOS 1.0+

``` source
func transform3DEffect(_ transform: AffineTransform3D) -> some VisualEffect
```

## Parameters 

`transform`  

The 3D transformation to apply to the view, interpreting it as a 3D plane in space.

## Return Value

An effect that renders transformed according to the provided `transform`

## See Also

### Applying a transform

func transformEffect(_:)

Applies an affine transformation to the view’s rendered output.

