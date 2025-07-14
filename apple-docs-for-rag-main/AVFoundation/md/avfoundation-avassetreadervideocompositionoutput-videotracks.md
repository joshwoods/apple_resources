

- AVFoundation
- AVAssetReaderVideoCompositionOutput
-  videoTracks 

Instance Property

# videoTracks

The tracks from which the output reads the composited video.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var videoTracks: [AVAssetTrack] { get }
```

## Discussion

The array contains AVAssetTrack objects owned by the target asset reader’s asset.

## See Also

### Inspecting an Output

var videoSettings: [String : Any]?

The video settings that the output uses.

