

- RealityKit
- TextureResource
- TextureResource.Semantic
-  TextureResource.Semantic.hdrColor 

Case

# TextureResource.Semantic.hdrColor

Use the texture to store a high-dynamic range image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case hdrColor
```

## Discussion

Properties that specify a semantic of `hdrColor` use the texture to store high-dynamic range RGB color data. If the source image contains color space information, RealityKit modifies the individual pixels to fit the color space. If the source image is grayscale, RealityKit converts it to an RGB image first.

## See Also

### Specifying intended use

case raw

Use the texture unmodified.

case color

Use the texture to store colors data.

case normal

Use the texture to store surface normals.

case scalar

Use the texture to store a single value in each pixel.

