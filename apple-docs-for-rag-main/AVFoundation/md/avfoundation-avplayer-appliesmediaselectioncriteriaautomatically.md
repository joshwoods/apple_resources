

- AVFoundation
- AVPlayer
-  appliesMediaSelectionCriteriaAutomatically 

Instance Property

# appliesMediaSelectionCriteriaAutomatically

A Boolean value that indicates whether the receiver should apply the current selection criteria automatically to player items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var appliesMediaSelectionCriteriaAutomatically: Bool { get set }
```

## Mentioned in 

Selecting Subtitles and Alternative Audio Tracks

## Discussion

By default, the `AVPlayer` instance applies selection criteria based on system accessibility preferences. To override the default criteria for any media selection group, use setMediaSelectionCriteria(_:forMediaCharacteristic:).

Note

For clients linked against the iOS 7.0 and later or against the macOS 10.9 and later, the default is true. For all others, the default is false.

## See Also

### Configuring Media Selection Criteria

func mediaSelectionCriteria(forMediaCharacteristic: AVMediaCharacteristic) -> AVPlayerMediaSelectionCriteria?

Returns the automatic selection criteria for media items with the specified media characteristic.

func setMediaSelectionCriteria(AVPlayerMediaSelectionCriteria?, forMediaCharacteristic: AVMediaCharacteristic)

Applies automatic selection criteria for media that has the specified media characteristic.

