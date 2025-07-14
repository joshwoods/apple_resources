

- UIKit
- UISwitch
-  init(frame:) 

Initializer

# init(frame:)

Creates a switch control.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(frame: CGRect)
```

## Parameters 

`frame`  

A rectangle defining the frame of the UISwitch object. The size components of this rectangle are ignored.

## Return Value

An initialized UISwitch object.

## Discussion

UISwitch overrides init(frame:) and enforces a size appropriate for the control.

## See Also

### Creating a switch

init?(coder: NSCoder)

Creates a switch control from data in an unarchiver.

