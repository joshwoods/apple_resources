

- RealityKit
- AudioFileResource
-  init(named:in:configuration:) 

Initializer

# init(named:in:configuration:)

Initializes an AudioFileResource asynchronously.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(
    named name: String,
    in bundle: Bundle? = nil,
    configuration: AudioFileResource.Configuration = .init()
) async throws
```

## Discussion

Important

The name provided **must** be unique.

## See Also

### Loading audio from a bundle

convenience init(named: String, from: String, in: Bundle?) async throws

Initializes a preconfigured AudioFileResource asynchronously from a Reality Composer Pro project with the given `name` as the the prim-path of the AudioFile, and the `scene` as the name of the USD file name.

