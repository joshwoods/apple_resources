

- RealityKit
- ARView
- ARView.Environment
-  ARView.Environment.ImageBasedLight 

Structure

# ARView.Environment.ImageBasedLight

Lighting properties of an environment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
struct ImageBasedLight
```

## Topics

### Resources

var resource: EnvironmentResource?

The resource containing lighting information for the image based light.

### Modulating intensity

var intensityExponent: Float

The intensity value of the light, defined on a logarithmic scale.

## See Also

### Lighting the environment

var lighting: ARView.Environment.ImageBasedLight

The lighting used in the environment of a particular scene.

