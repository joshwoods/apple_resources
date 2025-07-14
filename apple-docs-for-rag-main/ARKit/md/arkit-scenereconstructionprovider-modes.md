

- ARKit
- SceneReconstructionProvider
-  modes 

Instance Property

# modes

The modes of scene reconstruction a provider supplies.

visionOS 1.0+

``` source
final let modes: [SceneReconstructionProvider.Mode]
```

## See Also

### Creating a scene reconstruction provider

init(modes: [SceneReconstructionProvider.Mode])

Creates a provider that reconstructs a person’s surroundings.

enum Mode

The additional kinds of information you can request about a person’s surroundings.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports scene reconstruction providers.

