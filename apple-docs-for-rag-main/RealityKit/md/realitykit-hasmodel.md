

- RealityKit
-  HasModel 

Protocol

# HasModel

An interface that provides meshes and materials to define the visual appearance of an entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
protocol HasModel : HasTransform
```

## Topics

### Retrieving a model

var model: ModelComponent?

The model component for the entity.

### Managing joints

var jointNames: [String]

The names of all the joints in the model entity.

var jointTransforms: [Transform]

The relative joint transforms of the model entity.

### Instance Properties

var blendWeightNames: [[String]]

The names of the weights on each blend shape in the model entity.

var blendWeights: [[Float]]

The blend shape weights in the model entity.

var modelDebugOptions: ModelDebugOptionsComponent?

Configures the debug visualization of this model.

## Relationships

### Inherits From

- HasTransform

### Conforming Types

- BodyTrackedEntity
- ModelEntity

