

- ARKit
- SceneReconstructionProvider
-  init(modes:) 

Initializer

# init(modes:)

Creates a provider that reconstructs a person’s surroundings.

visionOS 1.0+

``` source
init(modes: [SceneReconstructionProvider.Mode] = [])
```

## Parameters 

`modes`  

The modes of scene reconstruction your app requires.

## Discussion

You can pass additional modes, such as SceneReconstructionProvider.Mode.classification, if you need more than the default mesh data.

## See Also

### Creating a scene reconstruction provider

let modes: [SceneReconstructionProvider.Mode]

The modes of scene reconstruction a provider supplies.

enum Mode

The additional kinds of information you can request about a person’s surroundings.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports scene reconstruction providers.

