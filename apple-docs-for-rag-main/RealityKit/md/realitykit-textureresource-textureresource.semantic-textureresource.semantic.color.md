

- RealityKit
- TextureResource
- TextureResource.Semantic
-  TextureResource.Semantic.color 

Case

# TextureResource.Semantic.color

Use the texture to store colors data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case color
```

## Discussion

Properties that specify a semantic of `color` use the RGB color data from the texture. If the source image contains color space information, RealityKit modifies the individual pixels to fit the color space. If the source image is grayscale, RealityKit converts it to an RGB image first.

## See Also

### Specifying intended use

case raw

Use the texture unmodified.

case hdrColor

Use the texture to store a high-dynamic range image.

case normal

Use the texture to store surface normals.

case scalar

Use the texture to store a single value in each pixel.

