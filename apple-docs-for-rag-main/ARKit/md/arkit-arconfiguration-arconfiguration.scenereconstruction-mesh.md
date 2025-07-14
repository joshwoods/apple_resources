

- ARKit
- ARConfiguration
- ARConfiguration.SceneReconstruction
-  mesh 

Type Property

# mesh

A polygonal mesh approximation of the physical environment.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
static var mesh: ARConfiguration.SceneReconstruction { get }
```

## See Also

### Modeling the Environment

init(rawValue: UInt)

Initializes a scene-reconstruction object.

static var meshWithClassification: ARConfiguration.SceneReconstruction

An approximate shape of the physical environment, including classification of the real-world objects within it.

