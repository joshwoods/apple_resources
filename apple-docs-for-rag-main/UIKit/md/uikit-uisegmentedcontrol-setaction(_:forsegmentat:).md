

- UIKit
- UISegmentedControl
-  setAction(\_:forSegmentAt:) 

Instance Method

# setAction(\_:forSegmentAt:)

Sets the action for the segment at the index you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func setAction(
    _ action: UIAction,
    forSegmentAt segment: Int
)
```

## Parameters 

`action`  

A UIAction object to set on the segment at the index you specify.

`segment`  

An integer index of a segment.

## Discussion

Segments prefer images over titles when the action contains both. Selecting a segment invokes the action’s UIActionHandler, as well as handlers for the valueChanged and primaryActionTriggered control events.

Note

This method asserts an error if the action’s UIAction.Identifier doesn’t match the action of the existing segment at this index, or isn’t unique within all actions associated with the segmented control.

## See Also

### Managing segment actions

func actionForSegment(at: Int) -> UIAction?

Fetches the action of the segment at the index you specify, if one exists.

