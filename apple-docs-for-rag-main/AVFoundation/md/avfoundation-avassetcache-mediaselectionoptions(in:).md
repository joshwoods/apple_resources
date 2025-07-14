

- AVFoundation
- AVAssetCache
-  mediaSelectionOptions(in:) 

Instance Method

# mediaSelectionOptions(in:)

Returns an array of locally cached media selection options that are available for offline use.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 10.0+

``` source
func mediaSelectionOptions(in mediaSelectionGroup: AVMediaSelectionGroup) -> [AVMediaSelectionOption]
```

## Parameters 

`mediaSelectionGroup`  

The containing media selection group.

## Return Value

The array of media selection options, or an empty array if none are available.

## See Also

### Inspecting the Cached Media

var isPlayableOffline: Bool

A Boolean value that indicates whether the asset is playable without an internet connection.

