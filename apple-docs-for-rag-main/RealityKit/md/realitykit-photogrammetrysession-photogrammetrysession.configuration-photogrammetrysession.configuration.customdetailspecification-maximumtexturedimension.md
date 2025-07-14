

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
- PhotogrammetrySession.Configuration.CustomDetailSpecification
-  maximumTextureDimension 

Instance Property

# maximumTextureDimension

The maximum dimension of the reconstructed texture maps.

Mac Catalyst 17.0+macOS 14.0+

``` source
var maximumTextureDimension: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureDimension
```

## Discussion

The reconstructed texture map will have width and height dimensions both less than or equal to the provided `maxTextureDimension`. This property is useful for fitting within the texture memory resources of the rendering system.

