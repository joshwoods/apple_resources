

- RealityKit
- AudioFileResource
- AudioFileResource.Configuration
-  shouldRandomizeStartTime 

Instance Property

# shouldRandomizeStartTime

Stores a Boolean indicating whether the playback begins from the start of the file, or from a random position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var shouldRandomizeStartTime: Bool
```

## Discussion

When this property and shouldLoop are both true, only the first playback iteration begins from a random position.

## See Also

### Customizing the playback

var shouldLoop: Bool

Stores a Boolean indicating whether the playback loops infinitely, until manually stopped or paused.

