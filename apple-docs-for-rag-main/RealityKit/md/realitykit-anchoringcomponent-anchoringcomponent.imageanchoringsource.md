

- RealityKit
- AnchoringComponent
-  AnchoringComponent.ImageAnchoringSource 

Structure

# AnchoringComponent.ImageAnchoringSource

Defines the source of object anchoring target based on how it is created.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ImageAnchoringSource
```

## Topics

### Operators

static func == (AnchoringComponent.ImageAnchoringSource, AnchoringComponent.ImageAnchoringSource) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(URL, physicalSize: SIMD2&lt;Float>)

Creates the image anchoring source from image file URL.

init(group: String, name: String)

Creates the image anchoring source by group and name in AR Resources.

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

struct ObjectAnchoringSource

Defines the source of object anchoring target based on how it is created.

