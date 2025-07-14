

- AVFoundation
- AVAssetReaderAudioMixOutput
-  audioSettings 

Instance Property

# audioSettings

The audio settings that the output uses.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var audioSettings: [String : Any]? { get }
```

## Discussion

The dictionary must contain values for the keys in Linear PCM Format Settings.

Setting the property value to `nil` indicates that the output returns audio samples in an uncompressed format.

## See Also

### Inspecting an Output

var audioTracks: [AVAssetTrack]

The tracks from which the output reads audio.

