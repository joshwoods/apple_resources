

- AVFoundation
- AVPlayer
-  setMediaSelectionCriteria(\_:forMediaCharacteristic:) 

Instance Method

# setMediaSelectionCriteria(\_:forMediaCharacteristic:)

Applies automatic selection criteria for media that has the specified media characteristic.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func setMediaSelectionCriteria(
    _ criteria: AVPlayerMediaSelectionCriteria?,
    forMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic
)
```

## Parameters 

`criteria`  

An instance of AVPlayerMediaSelectionCriteria that specifies the selection criteria.

`mediaCharacteristic`  

The media characteristic for which the selection criteria are to be applied. Supported values include audible, legible, and visual. See Media Characteristics in the `AVFoundation Constants`.

## Discussion

Criteria will be applied to an AVPlayerItem instance when:

- It is made ready to play.

- Specific media selections are made by the AVPlayerItem instance using the method select(_:in:) in a different group. The automatic choice in one group may be influenced by a specific selection in another group.

- Underlying system preferences change, e.g. system language, accessibility captions.

Specific selections made by the AVPlayerItem instance using the method select(_:in:) method within any group will override automatic selection in that group until the player item receives a selectMediaOptionAutomatically(in:) message.

## See Also

### Configuring Media Selection Criteria

var appliesMediaSelectionCriteriaAutomatically: Bool

A Boolean value that indicates whether the receiver should apply the current selection criteria automatically to player items.

func mediaSelectionCriteria(forMediaCharacteristic: AVMediaCharacteristic) -> AVPlayerMediaSelectionCriteria?

Returns the automatic selection criteria for media items with the specified media characteristic.

