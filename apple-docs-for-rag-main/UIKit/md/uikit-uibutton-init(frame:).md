

- UIKit
- UIButton
-  init(frame:) 

Initializer

# init(frame:)

Creates a new button with the specified frame.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(frame: CGRect)
```

## Parameters 

`frame`  

The frame rectangle for the view, measured in points.

## See Also

### Creating buttons

convenience init(frame: CGRect, primaryAction: UIAction?)

Creates a new button with the specified frame, registers the primary action event, and sets the title and image to the action’s title and image.

init?(coder: NSCoder)

Creates a new button with data in an unarchiver.

