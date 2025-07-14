

- UIKit
- UIEditMenuInteraction
-  reloadVisibleMenu() 

Instance Method

# reloadVisibleMenu()

Updates the actions an edit menu displays.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func reloadVisibleMenu()
```

## Discussion

You use this method to update the actions the menu displays. The method calls editMenuInteraction(_:menuFor:suggestedActions:) and updates the UI with the menu the delegate returns. The method has no effect if no menu is present.

## See Also

### Managing edit menu interactions

var delegate: (any UIEditMenuInteractionDelegate)?

An object that customizes presentation of the menu and actions to display for an edit menu interaction.

func presentEditMenu(with: UIEditMenuConfiguration)

Presents an edit menu using the object you provide for configuration.

func updateVisibleMenuPosition(animated: Bool)

Updates the position of the currently visible menu with an option to animate the action.

func dismissMenu()

Dismiss the edit menu if present.

func location(in: UIView?) -> CGPoint

Returns the location of the user interaction in the specified view’s coordinate system.

