

- Core Image
- CIRenderDestination
-  blendKernel 

Instance Property

# blendKernel

The destination's blend kernel.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var blendKernel: CIBlendKernel? { get set }
```

## See Also

### Customizing Rendering

var alphaMode: CIRenderDestinationAlphaMode

The render destination's representation of alpha (transparency) values.

enum CIRenderDestinationAlphaMode

Different ways of representing alpha.

var blendsInDestinationColorSpace: Bool

Indicator of whether to blend in the destination's color space.

var colorSpace: CGColorSpace?

The destination's color space.

var width: Int

The render destination's row width.

var height: Int

The render destination's buffer height.

var isClamped: Bool

Indicator of whether or not the destination clamps.

var isDithered: Bool

Indicator of whether or not the destination dithers.

var isFlipped: Bool

Indicator of whether the destination is flipped.

