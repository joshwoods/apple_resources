

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
- PhotogrammetrySession.Configuration.CustomDetailSpecification
-  outputTextureMaps 

Instance Property

# outputTextureMaps

The set of texture maps to create in the model.

Mac Catalyst 17.0+macOS 14.0+

``` source
var outputTextureMaps: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs
```

## Discussion

This setting can reduce model size by only requesting maps that will be used on the target renderer. Example to get just color and normal maps:

```
var detailSpec = PhotogrammetrySession.Request.Detail.Specification()
detailSpec.outputTextureMaps = [.diffuseColor, .normal]
```

