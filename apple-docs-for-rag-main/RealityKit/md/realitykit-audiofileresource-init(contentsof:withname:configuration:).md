

- RealityKit
- AudioFileResource
-  init(contentsOf:withName:configuration:) 

Initializer

# init(contentsOf:withName:configuration:)

Initializes an AudioFileResource asynchronously.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(
    contentsOf url: URL,
    withName resourceName: String? = nil,
    configuration: AudioFileResource.Configuration = .init()
) async throws
```

## Discussion

Important

The name provided **must** be unique.

