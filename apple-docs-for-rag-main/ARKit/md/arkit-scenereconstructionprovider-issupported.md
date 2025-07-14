

- ARKit
- SceneReconstructionProvider
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the current runtime environment supports scene reconstruction providers.

visionOS 1.0+

``` source
static var isSupported: Bool { get }
```

## See Also

### Creating a scene reconstruction provider

init(modes: [SceneReconstructionProvider.Mode])

Creates a provider that reconstructs a person’s surroundings.

let modes: [SceneReconstructionProvider.Mode]

The modes of scene reconstruction a provider supplies.

enum Mode

The additional kinds of information you can request about a person’s surroundings.

