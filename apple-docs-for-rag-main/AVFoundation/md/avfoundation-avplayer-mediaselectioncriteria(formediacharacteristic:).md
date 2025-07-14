

- AVFoundation
- AVPlayer
-  mediaSelectionCriteria(forMediaCharacteristic:) 

Instance Method

# mediaSelectionCriteria(forMediaCharacteristic:)

Returns the automatic selection criteria for media items with the specified media characteristic.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func mediaSelectionCriteria(forMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic) -> AVPlayerMediaSelectionCriteria?
```

## Parameters 

`mediaCharacteristic`  

The media characteristic for which the selection criteria is to be returned. Supported values include audible, legible, and visual.

## Return Value

The AVPlayerMediaSelectionCriteria for `mediaCharacteristic`.

## See Also

### Configuring Media Selection Criteria

var appliesMediaSelectionCriteriaAutomatically: Bool

A Boolean value that indicates whether the receiver should apply the current selection criteria automatically to player items.

func setMediaSelectionCriteria(AVPlayerMediaSelectionCriteria?, forMediaCharacteristic: AVMediaCharacteristic)

Applies automatic selection criteria for media that has the specified media characteristic.

