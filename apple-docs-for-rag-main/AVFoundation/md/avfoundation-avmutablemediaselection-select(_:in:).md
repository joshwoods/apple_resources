

- AVFoundation
- AVMutableMediaSelection
-  select(\_:in:) 

Instance Method

# select(\_:in:)

Selects the media option in the specified media selection group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func select(
    _ mediaSelectionOption: AVMediaSelectionOption?,
    in mediaSelectionGroup: AVMediaSelectionGroup
)
```

## Parameters 

`mediaSelectionOption`  

The media selection option to select.

`mediaSelectionGroup`  

The media selection group containing the specified media selection option.

## Discussion

This method selects the AVMediaSelectionOption in the specified AVMediaSelectionGroup and deselects all other options in that group. If the specified media selection option isn’t a member of the specified media selection group, no change in state will be made. If the media selection group’s allowsEmptySelection property is set to true, you can pass `nil` for `mediaSelectionOption` argument to deselect all media selection options in the group.

