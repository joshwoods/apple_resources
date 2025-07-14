

- RealityKit
- TextureResource
- TextureResource.Semantic
-  TextureResource.Semantic.normal 

Case

# TextureResource.Semantic.normal

Use the texture to store surface normals.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case normal
```

## Discussion

Properties that specify a semantic of `normal` use the texture to store tangent-space surface normal vectors for use in lighting calculations. Each pixel’s `R` channel stores the `X` value from the vector. The `G` channel stores the `Y` value from the vector, and the `B` channel stores the `Z` value from the vector. All values are between `-1.0` and `1.0`.

## See Also

### Specifying intended use

case raw

Use the texture unmodified.

case color

Use the texture to store colors data.

case hdrColor

Use the texture to store a high-dynamic range image.

case scalar

Use the texture to store a single value in each pixel.

