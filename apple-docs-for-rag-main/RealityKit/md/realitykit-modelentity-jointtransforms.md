

- RealityKit
- ModelEntity
-  jointTransforms 

Instance Property

# jointTransforms

The relative joint transforms of the model entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var jointTransforms: [Transform] { get set }
```

## Discussion

Call jointNames to determine the name and order of the joints.

Note

Active animations may override the joint transforms set using this property.

## See Also

### Configuring the model

var model: ModelComponent?

The model component for the entity.

var jointNames: [String]

The names of all the joints in the model entity.

