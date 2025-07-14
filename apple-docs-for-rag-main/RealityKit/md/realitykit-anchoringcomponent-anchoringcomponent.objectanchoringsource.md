

- RealityKit
- AnchoringComponent
-  AnchoringComponent.ObjectAnchoringSource 

Structure

# AnchoringComponent.ObjectAnchoringSource

Defines the source of object anchoring target based on how it is created.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ObjectAnchoringSource
```

## Topics

### Operators

static func == (AnchoringComponent.ObjectAnchoringSource, AnchoringComponent.ObjectAnchoringSource) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(URL)

Creates the object anchoring source by reference object file URL.

init(group: String, name: String)

Creates the object anchoring source by group and name in AR Resources.

init(name: String, in: Bundle)

Creates the object anchoring source by reference object file asset with provided name and bundle.

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

- Equatable
- Hashable

## See Also

### Image and object tracking

struct ImageAnchoringSource

Defines the source of object anchoring target based on how it is created.

