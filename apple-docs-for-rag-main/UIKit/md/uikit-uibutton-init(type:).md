

- UIKit
- UIButton
-  init(type:) 

Initializer

# init(type:)

Creates and returns a new button of the specified type.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(type buttonType: UIButton.ButtonType)
```

## Parameters 

`buttonType`  

The button type. See UIButton.ButtonType for the possible values.

## Return Value

A newly created button.

## Discussion

This method is a convenience constructor for creating button objects with specific configurations.

When creating a custom button — a button with the type UIButton.ButtonType.custom — the frame of the button is set to (`0`, `0`, `0`, `0`) initially. Before adding the button to your interface, you should update the frame to a more appropriate value.

## See Also

### Related Documentation

UIKit Catalog: Creating and customizing views and controls

Customize your app’s user interface with views and controls.

### Creating buttons of a specific type

convenience init(type: UIButton.ButtonType, primaryAction: UIAction?)

Creates a new button with the specified type, registers the primary action event, and sets the title and image to the action’s title and image.

enum ButtonType

Specifies the style of a button.

