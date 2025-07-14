

- UIKit
- UIEditMenuInteraction
-  presentEditMenu(with:) 

Instance Method

# presentEditMenu(with:)

Presents an edit menu using the object you provide for configuration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func presentEditMenu(with configuration: UIEditMenuConfiguration)
```

## Parameters 

`configuration`  

The object containing the configuration details for the menu.

## Discussion

You use this method to display the edit menu. The method calls editMenuInteraction(_:menuFor:suggestedActions:) on the interaction object’s delegate and updates the UI with the menu the delegate returns. This method dismisses any active menus before presenting the new menu.

The following example presents the menu from a gesture recognizer and provides the location of the gesture as the location for this interaction.

```
    @objc func didLongPress(_ recognizer: UIGestureRecognizer) {
        let location = recognizer.location(in: self.view)
        let configuration = UIEditMenuConfiguration(identifier: nil, sourcePoint: location)

        if let interaction = editMenuInteraction {
            // Presenting the edit menu interaction
            interaction.presentEditMenu(with: configuration)
        }
    }
```

## See Also

### Managing edit menu interactions

var delegate: (any UIEditMenuInteractionDelegate)?

An object that customizes presentation of the menu and actions to display for an edit menu interaction.

func reloadVisibleMenu()

Updates the actions an edit menu displays.

func updateVisibleMenuPosition(animated: Bool)

Updates the position of the currently visible menu with an option to animate the action.

func dismissMenu()

Dismiss the edit menu if present.

func location(in: UIView?) -> CGPoint

Returns the location of the user interaction in the specified view’s coordinate system.

