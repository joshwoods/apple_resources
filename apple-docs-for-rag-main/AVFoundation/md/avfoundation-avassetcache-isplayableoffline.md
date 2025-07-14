

- AVFoundation
- AVAssetCache
-  isPlayableOffline 

Instance Property

# isPlayableOffline

A Boolean value that indicates whether the asset is playable without an internet connection.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 10.0+

``` source
var isPlayableOffline: Bool { get }
```

## Discussion

Check the value of this property to determine the asset’s suitability for playback before presenting or attempting to play it.

Note

A property value of true doesn’t indicate that all of the asset’s associated media selection options are available for offline playback. Instead, call mediaSelectionOptions(in:) to determine which media selections are available.

## See Also

### Inspecting the Cached Media

func mediaSelectionOptions(in: AVMediaSelectionGroup) -> [AVMediaSelectionOption]

Returns an array of locally cached media selection options that are available for offline use.

