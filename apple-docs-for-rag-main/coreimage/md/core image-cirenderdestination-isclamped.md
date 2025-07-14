

- Core Image
- CIRenderDestination
-  isClamped 

Instance Property

# isClamped

Indicator of whether or not the destination clamps.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var isClamped: Bool { get set }
```

## See Also

### Customizing Rendering

var alphaMode: CIRenderDestinationAlphaMode

The render destination's representation of alpha (transparency) values.

enum CIRenderDestinationAlphaMode

Different ways of representing alpha.

var blendKernel: CIBlendKernel?

The destination's blend kernel.

var blendsInDestinationColorSpace: Bool

Indicator of whether to blend in the destination's color space.

var colorSpace: CGColorSpace?

The destination's color space.

var width: Int

The render destination's row width.

var height: Int

The render destination's buffer height.

var isDithered: Bool

Indicator of whether or not the destination dithers.

var isFlipped: Bool

Indicator of whether the destination is flipped.

