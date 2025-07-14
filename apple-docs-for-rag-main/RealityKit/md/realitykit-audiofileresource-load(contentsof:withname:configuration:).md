

- RealityKit
- AudioFileResource
-  load(contentsOf:withName:configuration:) 

Type Method

# load(contentsOf:withName:configuration:)

Loads an AudioFileResource synchronously.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static func load(
    contentsOf url: URL,
    withName name: String? = nil,
    configuration: AudioFileResource.Configuration = .init()
) throws -> AudioFileResource
```

## Discussion

Important

The name provided **must** be unique.

