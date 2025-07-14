

- RealityKit
- AudioFileResource
-  load(named:from:in:) 

Type Method

# load(named:from:in:)

Loads a preconfigured AudioFileResource from a Reality Composer Pro project with the given `name` as the the prim-path of the AudioFile, and the `scene` as the name of the USD file name.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static func load(
    named name: String,
    from scene: String,
    in bundle: Bundle? = nil
) throws -> AudioFileResource
```

## Discussion

Important

The name provided **must** be unique.

