

- UIKit
- UIEditMenuInteraction
-  updateVisibleMenuPosition(animated:) 

Instance Method

# updateVisibleMenuPosition(animated:)

Updates the position of the currently visible menu with an option to animate the action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func updateVisibleMenuPosition(animated: Bool)
```

## Parameters 

`animated`  

`YES` to animate the transition to the new position; `NO` to make the transition immediate.

## Discussion

You use this method to update the location of the menu. This method calls editMenuInteraction(_:targetRectFor:) and updates the position of the menu using the position the delegate returns. The method has no effect if no menu is present.

## See Also

### Managing edit menu interactions

var delegate: (any UIEditMenuInteractionDelegate)?

An object that customizes presentation of the menu and actions to display for an edit menu interaction.

func presentEditMenu(with: UIEditMenuConfiguration)

Presents an edit menu using the object you provide for configuration.

func reloadVisibleMenu()

Updates the actions an edit menu displays.

func dismissMenu()

Dismiss the edit menu if present.

func location(in: UIView?) -> CGPoint

Returns the location of the user interaction in the specified view’s coordinate system.

