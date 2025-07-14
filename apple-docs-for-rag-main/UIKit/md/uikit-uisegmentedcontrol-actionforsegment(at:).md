

- UIKit
- UISegmentedControl
-  actionForSegment(at:) 

Instance Method

# actionForSegment(at:)

Fetches the action of the segment at the index you specify, if one exists.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func actionForSegment(at segment: Int) -> UIAction?
```

## Parameters 

`segment`  

An integer value index of a segment.

## Return Value

The UIAction for the segment at the index you specify, or `nil` if the segment doesn’t have an action assigned.

## See Also

### Managing segment actions

func setAction(UIAction, forSegmentAt: Int)

Sets the action for the segment at the index you specify.

