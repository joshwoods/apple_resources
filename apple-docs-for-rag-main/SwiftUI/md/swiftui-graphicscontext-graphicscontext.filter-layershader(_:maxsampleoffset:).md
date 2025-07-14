

- SwiftUI
- GraphicsContext
- GraphicsContext.Filter
-  layerShader(\_:maxSampleOffset:) 

Type Method

# layerShader(\_:maxSampleOffset:)

Returns a filter that applies `shader` to the contents of the source layer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
static func layerShader(
    _ shader: Shader,
    maxSampleOffset: CGSize
) -> GraphicsContext.Filter
```

## Parameters 

`shader`  

The shader to apply as a layer effect.

`maxSampleOffset`  

If the shader function samples from the layer at locations not equal to the destination position, this value must specify the maximum sampling distance in each axis, for all source pixels.

## Return Value

A filter applies the shader as a layer effect.

## Discussion

For a shader function to act as a layer effect it must have a function signature matching:

```
[[ stitchable ]] half4 name(float2 position,
  SwiftUI::Layer layer, args...)
```

where `position` is the user-space coordinates of the destination pixel applied to the shader, and `layer` is a rasterized subregion of the source layer. `args...` should be compatible with the uniform arguments bound to `shader`.

The `SwiftUI::Layer` type is defined in the `` header file. It exports a single `sample()` function that returns a linearly-filtered pixel value from a position in the source content, as a premultiplied RGBA pixel value:

```
namespace SwiftUI {
  struct Layer {
    half4 sample(float2 position) const;
  };
};
```

The function should return the color mapping to the destination pixel, typically by sampling one or more pixels from `layer` at location(s) derived from `position` and them applying some kind of transformation to produce a new color.

## See Also

### Using a custom Metal shader

static func colorShader(Shader) -> GraphicsContext.Filter

Returns a filter that applies `shader` to the color of each source pixel.

static func distortionShader(Shader, maxSampleOffset: CGSize) -> GraphicsContext.Filter

Returns a filter that applies `shader` as a geometric distortion effect on the location of each pixel.

