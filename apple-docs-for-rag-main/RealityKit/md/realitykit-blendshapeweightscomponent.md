

- RealityKit
-  BlendShapeWeightsComponent 

Structure

# BlendShapeWeightsComponent

A component that provides access to the current weights associated with all blend shape meshes on an entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct BlendShapeWeightsComponent
```

## Overview

You can access the weights associated with an entity’s blend shapes by using the weightSet variable after an initialized `BlendShapeWeightsComponent` is added to an entity.

```
let blendShapeWeightsComponent = BlendShapeWeightsComponent(
    weightsMapping: weightsMapping)
entity.components.set(blendShapeWeightsComponent)
let weightValues: [Float] = [0.3, 0.8]
entity.components[BlendShapeWeightsComponent.self]!.weightSets[0].weights
    = weightValues
```

## Topics

### Initializers

init(weightsMapping: BlendShapeWeightsMapping)

Create a BlendShapeWeightsComponent from a BlendShapeWeightsMapping.

### Instance Properties

var weightSet: BlendShapeWeightsSet

The runtime named blend shapes weights.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Blend shape management

class BlendShapeWeightsMapping

A mapping of blend weights to the target meshes that those weights affect.

struct BlendShapeWeights

A set of animatable weight values that collectively represent the blending amounts for all the blend shapes’ blend targets.

struct BlendShapeWeightsData

A structure that encapsulates the blend shape name, blend shape weights and the names of those weights to be stored by the blend shape weights set.

struct BlendShapeWeightsSet

A custom collection of named blend shape weights.

