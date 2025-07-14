

- Cinematic
- CNScript
-  init(asset:changes:progress:) 

Initializer

# init(asset:changes:progress:)

Creates a Cinematic script based on a movie and applying changes to the movie.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
init(
    asset: AVAsset,
    changes: CNScript.Changes? = nil,
    progress: Progress? = nil
) async throws
```

## Parameters 

`asset`  

The original movie.

`changes`  

Changes to apply to the original script.

`progress`  

The optional progress object to track progress or cancel loading.

