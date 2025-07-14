

- AVFoundation
- AVPlayerItem
-  select(\_:in:) 

Instance Method

# select(\_:in:)

Selects a media option in a given media selection group and deselects all other options in that group.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func select(
    _ mediaSelectionOption: AVMediaSelectionOption?,
    in mediaSelectionGroup: AVMediaSelectionGroup
)
```

## Parameters 

`mediaSelectionOption`  

The option to select.

If the value of the allowsEmptySelection property of `mediaSelectionGroup` is true, you can pass `nil` to deselect all media selection options in the group.

`mediaSelectionGroup`  

The media selection group, obtained from the receiver’s asset, that contains `mediaSelectionOption`.

## Mentioned in 

Selecting Subtitles and Alternative Audio Tracks

## Discussion

If `mediaSelectionOption` isn’t a member of the `mediaSelectionGroup`, no change in presentation state will result.

If multiple options within a group meet your criteria for selection according to locale or other considerations, and if these options are otherwise indistinguishable to you according to media characteristics that are meaningful for your application, content is typically authored so that the first available option that meets your criteria is appropriate for selection.

## See Also

### Selecting Media Options

var currentMediaSelection: AVMediaSelection

The current media selections for each of the receiver’s media selection groups.

func selectMediaOptionAutomatically(in: AVMediaSelectionGroup)

Selects the media option in the specified media selection group that best matches the receiver’s automatic selection criteria.

