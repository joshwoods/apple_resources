

- UIKit
- UISegmentedControl
-  init(frame:actions:) 

Initializer

# init(frame:actions:)

Creates a segmented control with the given frame and adds segments for the actions you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    frame: CGRect,
    actions: [UIAction]
)
```

## Parameters 

`frame`  

A rectangle that specifies the segmented control’s frame in a superview’s coordinate system.

`actions`  

An array of UIAction objects.

## Discussion

Segments prefer images over titles when the action contains both. Selecting a segment invokes the action’s UIActionHandler, as well as handlers for the valueChanged and primaryActionTriggered control events.

## See Also

### Creating a segmented control

init(items: [Any]?)

Creates a segmented control with segments having the given titles or images.

init(frame: CGRect)

Creates an empty segmented control with the frame you specify.

init?(coder: NSCoder)

Creates a segmented control with data from an unarchiver.

