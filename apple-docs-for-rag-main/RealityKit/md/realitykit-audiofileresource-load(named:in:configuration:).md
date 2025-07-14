

- RealityKit
- AudioFileResource
-  load(named:in:configuration:) 

Type Method

# load(named:in:configuration:)

Loads an AudioFileResource synchronously.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static func load(
    named name: String,
    in bundle: Bundle? = nil,
    configuration: AudioFileResource.Configuration = .init()
) throws -> AudioFileResource
```

## Discussion

Important

The name provided **must** be unique.

