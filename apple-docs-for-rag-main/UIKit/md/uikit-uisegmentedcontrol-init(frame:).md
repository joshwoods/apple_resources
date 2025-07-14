

- UIKit
- UISegmentedControl
-  init(frame:) 

Initializer

# init(frame:)

Creates an empty segmented control with the frame you specify.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(frame: CGRect)
```

## Parameters 

`frame`  

A rectangle that specifies the segmented control’s frame in a superview’s coordinate system.

## See Also

### Creating a segmented control

init(items: [Any]?)

Creates a segmented control with segments having the given titles or images.

convenience init(frame: CGRect, actions: [UIAction])

Creates a segmented control with the given frame and adds segments for the actions you specify.

init?(coder: NSCoder)

Creates a segmented control with data from an unarchiver.

