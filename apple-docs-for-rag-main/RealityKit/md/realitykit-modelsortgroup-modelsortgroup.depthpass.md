

- RealityKit
- ModelSortGroup
-  ModelSortGroup.DepthPass 

Enumeration

# ModelSortGroup.DepthPass

Options that indicate when the renderer draws a model’s depth relative to its color.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum DepthPass
```

## Topics

### Operators

static func == (ModelSortGroup.DepthPass, ModelSortGroup.DepthPass) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case postPass

An option that instructs the renderer to draw the depth of a model only after it draws the colors for all the models in the group first.

case prePass

An option that instructs the renderer to draw the depth of all the models in the group before it draws any model’s color.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

