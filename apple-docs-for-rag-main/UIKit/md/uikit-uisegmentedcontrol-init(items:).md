

- UIKit
- UISegmentedControl
-  init(items:) 

Initializer

# init(items:)

Creates a segmented control with segments having the given titles or images.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(items: [Any]?)
```

## Parameters 

`items`  

An array of NSString objects (for segment titles), UIImage objects (for segment images), or in iOS 14.0 and later UIAction objects.

## Return Value

A `UISegmentedControl` object or `nil` if there was a problem in initializing the object.

## Discussion

The system automatically sizes the returned segmented control to fit its content within the width of its superview.

## See Also

### Creating a segmented control

convenience init(frame: CGRect, actions: [UIAction])

Creates a segmented control with the given frame and adds segments for the actions you specify.

init(frame: CGRect)

Creates an empty segmented control with the frame you specify.

init?(coder: NSCoder)

Creates a segmented control with data from an unarchiver.

