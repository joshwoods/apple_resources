

- RealityKit
- TextureResource
- TextureResource.Semantic
-  TextureResource.Semantic.raw 

Case

# TextureResource.Semantic.raw

Use the texture unmodified.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case raw
```

## Discussion

For texture properties that use the `raw` semantic, the number of channels and values is the same as the source image. If the source image contains color space information, RealityKit ignores it. For `raw` textures, each individual pixel contains one floating-point value between `0.0` and `1.0` for each channel in the source image. For example, a grayscale source image results in a texture that contains one value per pixel, and an RGB source image results in three values per pixel.

## See Also

### Specifying intended use

case color

Use the texture to store colors data.

case hdrColor

Use the texture to store a high-dynamic range image.

case normal

Use the texture to store surface normals.

case scalar

Use the texture to store a single value in each pixel.

