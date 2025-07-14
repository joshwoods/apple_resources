

- RealityKit
-  BlendShapeWeightsData 

Structure

# BlendShapeWeightsData

A structure that encapsulates the blend shape name, blend shape weights and the names of those weights to be stored by the blend shape weights set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct BlendShapeWeightsData
```

## Topics

### Initializers

init(id: BlendShapeWeightsData.ID, weights: [(String, BlendShapeWeights.Element)])

Creates an instance of the named weights for a single blend shape.

### Instance Properties

var id: BlendShapeWeightsData.ID

The unique id of the blend shape. This value is used when binding to the structure using an animation bind target.

var weightNames: [String]

The name of each weight value defined in the weights variable.

var weights: BlendShapeWeights

The blend shape’s weight values.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable

## See Also

### Blend shape management

struct BlendShapeWeightsComponent

A component that provides access to the current weights associated with all blend shape meshes on an entity.

class BlendShapeWeightsMapping

A mapping of blend weights to the target meshes that those weights affect.

struct BlendShapeWeights

A set of animatable weight values that collectively represent the blending amounts for all the blend shapes’ blend targets.

struct BlendShapeWeightsSet

A custom collection of named blend shape weights.

