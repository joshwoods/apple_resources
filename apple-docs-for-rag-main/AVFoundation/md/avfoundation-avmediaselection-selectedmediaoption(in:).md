

- AVFoundation
- AVMediaSelection
-  selectedMediaOption(in:) 

Instance Method

# selectedMediaOption(in:)

Returns the media selection option that’s currently selected in the specified group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func selectedMediaOption(in mediaSelectionGroup: AVMediaSelectionGroup) -> AVMediaSelectionOption?
```

## Parameters 

`mediaSelectionGroup`  

A media selection group obtained from the associated asset.

## Return Value

The currently selected AVMediaSelectionOption. The return value may be `nil`.

## Discussion

This method returns the currently selected AVMediaSelectionOption in the specified AVMediaSelectionGroup, but may return `nil` if media selection group’s allowsEmptySelection is set to true.

## See Also

### Inspecting the Media Selection

func mediaSelectionCriteriaCanBeAppliedAutomatically(to: AVMediaSelectionGroup) -> Bool

Indicates whether the specified media selection group is subject to automatic media selection.

