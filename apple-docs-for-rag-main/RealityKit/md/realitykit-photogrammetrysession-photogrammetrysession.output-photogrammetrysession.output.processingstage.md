

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Output
-  PhotogrammetrySession.Output.ProcessingStage 

Enumeration

# PhotogrammetrySession.Output.ProcessingStage

Processing stages during reconstruction.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
enum ProcessingStage
```

## Topics

### Operators

static func == (PhotogrammetrySession.Output.ProcessingStage, PhotogrammetrySession.Output.ProcessingStage) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case imageAlignment

case meshGeneration

case optimization

case pointCloudGeneration

case preProcessing

case textureMapping

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

