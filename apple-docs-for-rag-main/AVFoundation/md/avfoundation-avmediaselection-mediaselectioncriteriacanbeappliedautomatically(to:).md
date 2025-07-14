

- AVFoundation
- AVMediaSelection
-  mediaSelectionCriteriaCanBeAppliedAutomatically(to:) 

Instance Method

# mediaSelectionCriteriaCanBeAppliedAutomatically(to:)

Indicates whether the specified media selection group is subject to automatic media selection.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func mediaSelectionCriteriaCanBeAppliedAutomatically(to mediaSelectionGroup: AVMediaSelectionGroup) -> Bool
```

## Parameters 

`mediaSelectionGroup`  

A media selection group obtained from the associated asset.

## Return Value

A Boolean value indicating whether the group is subject to automatic media selection.

## Discussion

The automatic application of media selection criteria is suspended in any group in which a specific selection has been made by calling select(_:in:) on the current AVPlayerItem.

## See Also

### Inspecting the Media Selection

func selectedMediaOption(in: AVMediaSelectionGroup) -> AVMediaSelectionOption?

Returns the media selection option that’s currently selected in the specified group.

