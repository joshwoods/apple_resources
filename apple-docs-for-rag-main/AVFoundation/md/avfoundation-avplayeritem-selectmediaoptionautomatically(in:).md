

- AVFoundation
- AVPlayerItem
-  selectMediaOptionAutomatically(in:) 

Instance Method

# selectMediaOptionAutomatically(in:)

Selects the media option in the specified media selection group that best matches the receiver’s automatic selection criteria.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func selectMediaOptionAutomatically(in mediaSelectionGroup: AVMediaSelectionGroup)
```

## Parameters 

`mediaSelectionGroup`  

The media selection group, obtained from the receiver’s asset, that contains the specified option.

## Discussion

This method has no effect unless the appliesMediaSelectionCriteriaAutomatically property of the associated AVPlayer is true and unless automatic media selection has previously been overridden by invoking select(_:in:).

## See Also

### Selecting Media Options

var currentMediaSelection: AVMediaSelection

The current media selections for each of the receiver’s media selection groups.

func select(AVMediaSelectionOption?, in: AVMediaSelectionGroup)

Selects a media option in a given media selection group and deselects all other options in that group.

