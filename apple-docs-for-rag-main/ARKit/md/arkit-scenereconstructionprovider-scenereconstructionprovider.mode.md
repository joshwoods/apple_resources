

- ARKit
- SceneReconstructionProvider
-  SceneReconstructionProvider.Mode 

Enumeration

# SceneReconstructionProvider.Mode

The additional kinds of information you can request about a person’s surroundings.

visionOS 1.0+

``` source
enum Mode
```

## Topics

### Scene reconstruction modes

case classification

The reconstruction mode that classifies each face of a mesh anchor.

### Instance Properties

var description: String

A textual representation of SceneReconstructionProvider.Mode

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Creating a scene reconstruction provider

init(modes: [SceneReconstructionProvider.Mode])

Creates a provider that reconstructs a person’s surroundings.

let modes: [SceneReconstructionProvider.Mode]

The modes of scene reconstruction a provider supplies.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports scene reconstruction providers.

