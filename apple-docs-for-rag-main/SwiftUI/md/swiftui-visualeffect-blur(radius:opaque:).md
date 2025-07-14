

- SwiftUI
- VisualEffect
-  blur(radius:opaque:) 

Instance Method

# blur(radius:opaque:)

Applies a Gaussian blur to the view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func blur(
    radius: CGFloat,
    opaque: Bool = false
) -> some VisualEffect
```

## Parameters 

`radius`  

The radial size of the blur. A blur is more diffuse when its radius is large.

`opaque`  

A Boolean value that indicates whether the blur renderer permits transparency in the blur output. Set to `true` to create an opaque blur, or set to `false` to permit transparency.

## Return Value

An effect that blurs the view.

## Discussion

Use `blur(radius:opaque:)` to apply a gaussian blur effect to the rendering of the view.

## See Also

### Applying other effects

func distortionEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some VisualEffect

Returns a new visual effect that applies `shader` to `self` as a geometric distortion effect on the location of each pixel.

func layerEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some VisualEffect

Returns a new visual effect that applies `shader` to `self` as a filter on the raster layer created from `self`.

