

- UIKit
- UIEditMenuInteraction
-  dismissMenu() 

Instance Method

# dismissMenu()

Dismiss the edit menu if present.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func dismissMenu()
```

## Discussion

You use this method to dismiss the menu, for example, from an observer callback in your app.

## See Also

### Managing edit menu interactions

var delegate: (any UIEditMenuInteractionDelegate)?

An object that customizes presentation of the menu and actions to display for an edit menu interaction.

func presentEditMenu(with: UIEditMenuConfiguration)

Presents an edit menu using the object you provide for configuration.

func reloadVisibleMenu()

Updates the actions an edit menu displays.

func updateVisibleMenuPosition(animated: Bool)

Updates the position of the currently visible menu with an option to animate the action.

func location(in: UIView?) -> CGPoint

Returns the location of the user interaction in the specified view’s coordinate system.

