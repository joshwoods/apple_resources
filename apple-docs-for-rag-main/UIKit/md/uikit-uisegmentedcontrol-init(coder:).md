

- UIKit
- UISegmentedControl
-  init(coder:) 

Initializer

# init(coder:)

Creates a segmented control with data from an unarchiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## Parameters 

`coder`  

The unarchiver to read data from.

## See Also

### Creating a segmented control

init(items: [Any]?)

Creates a segmented control with segments having the given titles or images.

convenience init(frame: CGRect, actions: [UIAction])

Creates a segmented control with the given frame and adds segments for the actions you specify.

init(frame: CGRect)

Creates an empty segmented control with the frame you specify.

