

- UIKit
- UIButton
-  init(frame:primaryAction:) 

Initializer

# init(frame:primaryAction:)

Creates a new button with the specified frame, registers the primary action event, and sets the title and image to the action’s title and image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    frame: CGRect,
    primaryAction: UIAction?
)
```

## Parameters 

`frame`  

The frame rectangle for the view, measured in points.

`primaryAction`  

The action to perform when the button is selected. The button registers this action for the primaryActionTriggered control event and sets the title and image properties to the action’s title and image.

## See Also

### Creating buttons

init(frame: CGRect)

Creates a new button with the specified frame.

init?(coder: NSCoder)

Creates a new button with data in an unarchiver.

