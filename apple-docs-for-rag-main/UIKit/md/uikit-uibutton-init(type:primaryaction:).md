

- UIKit
- UIButton
-  init(type:primaryAction:) 

Initializer

# init(type:primaryAction:)

Creates a new button with the specified type, registers the primary action event, and sets the title and image to the action’s title and image.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    type buttonType: UIButton.ButtonType = .system,
    primaryAction: UIAction?
)
```

## Parameters 

`buttonType`  

The type of button.

`primaryAction`  

The action to perform when the button is selected. The button registers this action for the primaryActionTriggered control event and sets the title and image properties to the action’s title and image.

## See Also

### Creating buttons of a specific type

convenience init(type: UIButton.ButtonType)

Creates and returns a new button of the specified type.

enum ButtonType

Specifies the style of a button.

