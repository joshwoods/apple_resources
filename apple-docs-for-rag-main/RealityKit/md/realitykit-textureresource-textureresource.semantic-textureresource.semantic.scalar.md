

- RealityKit
- TextureResource
- TextureResource.Semantic
-  TextureResource.Semantic.scalar 

Case

# TextureResource.Semantic.scalar

Use the texture to store a single value in each pixel.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case scalar
```

## Discussion

Properties that specify a semantic of `scalar` use the texture to store a single floating point value in each pixel. If the texture’s source is an RGB image, the property uses only the red channel value.

## See Also

### Specifying intended use

case raw

Use the texture unmodified.

case color

Use the texture to store colors data.

case hdrColor

Use the texture to store a high-dynamic range image.

case normal

Use the texture to store surface normals.

