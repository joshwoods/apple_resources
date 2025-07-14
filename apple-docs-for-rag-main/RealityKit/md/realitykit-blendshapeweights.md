

- RealityKit
-  BlendShapeWeights 

Structure

# BlendShapeWeights

A set of animatable weight values that collectively represent the blending amounts for all the blend shapes’ blend targets.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct BlendShapeWeights
```

## Topics

### Operators

static func == (BlendShapeWeights, BlendShapeWeights) -> Bool

Returns a Boolean value that indicates whether two collections of weights are equal.

### Initializers

init()

Initializes a collection of animatable weights for a blend shape.

init&lt;S>(S)

Initializes a collection of weights for a single blend shape.

init(arrayLiteral: Float...)

Creates a collection of animatable weights using the argument elements for a blend shape.

### Instance Properties

var endIndex: BlendShapeWeights.Index

An index to the last weight in the collection.

var startIndex: BlendShapeWeights.Index

An index to the first weight in the collection.

### Instance Methods

func index(after: BlendShapeWeights.Index) -> BlendShapeWeights.Index

Returns the position in the sequence of the weight that follows the given position.

func index(before: BlendShapeWeights.Index) -> BlendShapeWeights.Index

Returns the position in the sequence of the weight that preceeds the given position.

### Subscripts

subscript(BlendShapeWeights.Index) -> Float

Accesses a single weight in the collection at the given index.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

An individual weight in the collection.

typealias Index

A position of an individual weight in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

MutableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- AnimatableData
- BidirectionalCollection
- Collection
- Copyable
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- MutableCollection
- Sequence

## See Also

### Blend shape management

struct BlendShapeWeightsComponent

A component that provides access to the current weights associated with all blend shape meshes on an entity.

class BlendShapeWeightsMapping

A mapping of blend weights to the target meshes that those weights affect.

struct BlendShapeWeightsData

A structure that encapsulates the blend shape name, blend shape weights and the names of those weights to be stored by the blend shape weights set.

struct BlendShapeWeightsSet

A custom collection of named blend shape weights.

