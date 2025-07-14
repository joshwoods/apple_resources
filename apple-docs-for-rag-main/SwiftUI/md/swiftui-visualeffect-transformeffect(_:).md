

- SwiftUI
- VisualEffect
-  transformEffect(\_:) 

Instance Method

# transformEffect(\_:)

Applies an affine transformation to the view’s rendered output.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func transformEffect(_ transform: CGAffineTransform) -> some VisualEffect
```

Show all declarations

## Parameters 

`transform`  

A CGAffineTransform to apply to the view.

## Return Value

An effect that applies an affine transformation to the view’s rendered output.

## Discussion

Use `transformEffect(_:)` to rotate, scale, translate, or skew the output of the view according to the provided CGAffineTransform.

## See Also

### Applying a transform

func transform3DEffect(AffineTransform3D) -> some VisualEffect

Applies a 3D transformation to the receiver.

