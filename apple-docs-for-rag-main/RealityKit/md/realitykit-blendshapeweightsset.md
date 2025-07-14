

- RealityKit
-  BlendShapeWeightsSet 

Structure

# BlendShapeWeightsSet

A custom collection of named blend shape weights.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct BlendShapeWeightsSet
```

## Overview

Retrieve a `BlendShapeWeightsSet` from a BlendShapeWeightsComponent to access the current weights and weight names for each blend shape managed by the component.

Set the current weights for a blend shape by assigning a `BlendShapeWeightsSet` to a BlendShapeWeightsComponent for a specific blend shape.

The collection allows:

- Access to elements by name.

- Protection that prohibits updating an element, where such an update would try to rename the stored element.

BlendShapeWeightsSet does not support addition/removal of elements, as the blend shape weights are defined in the asset and the number and names of the weights are immutable.

## Topics

### Initializers

init()

Creates an empty set.

### Instance Properties

var count: Int

Number of blend shape weight data in the set.

var `default`: BlendShapeWeightsSet.Element?

The blend shape weights data set that drives the model.

var isEmpty: Bool

Checks if the set contains any blend shape weights data.

### Instance Methods

func contains(String) -> Bool

Checks if the set contains a blend shape weights data instance with the given name.

func index(of: String) -> BlendShapeWeightsSet.Index?

Returns the index where the specified blend shape weights data appears in the collection.

func set(BlendShapeWeightsSet.Element) -> BlendShapeWeightsSet.Element?

Updates a blend shape weights data instance in the set based on its name. If blend shape weights data with this ID does not exist, does nothing.

### Subscripts

subscript(String) -> BlendShapeWeightsSet.Element?

Accessor for reading a blend shape weights data in the set.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

### Default Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable
- Sequence

## See Also

### Blend shape management

struct BlendShapeWeightsComponent

A component that provides access to the current weights associated with all blend shape meshes on an entity.

class BlendShapeWeightsMapping

A mapping of blend weights to the target meshes that those weights affect.

struct BlendShapeWeights

A set of animatable weight values that collectively represent the blending amounts for all the blend shapes’ blend targets.

struct BlendShapeWeightsData

A structure that encapsulates the blend shape name, blend shape weights and the names of those weights to be stored by the blend shape weights set.

