

- RealityKit
- AudioFileGroupResource
-  init(\_:) 

Initializer

# init(\_:)

Creates a group resource from an array of audio file resources.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
init(_ resources: [AudioFileResource]) throws
```

## Discussion

An AudioFileGroupResource provides a single, random element from its collection of AudioFileResource objects each time play() is called on the AudioPlaybackController on which it is prepared.

Throws

An error if the provided array is empty or if the underlying audio assets do not have matching channel layouts.

## See Also

### Creating a resource

convenience init(named: String, from: String, in: Bundle) async throws

Initializes an audio resource from a Reality Composer Pro project.

static func load(named: String, from: String, in: Bundle?) throws -> AudioFileGroupResource

Loads an audio resource from a Reality Composer Pro project.

