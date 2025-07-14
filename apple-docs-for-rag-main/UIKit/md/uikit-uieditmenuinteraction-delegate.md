

- UIKit
- UIEditMenuInteraction
-  delegate 

Instance Property

# delegate

An object that customizes presentation of the menu and actions to display for an edit menu interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIEditMenuInteractionDelegate)? { get }
```

## See Also

### Managing edit menu interactions

func presentEditMenu(with: UIEditMenuConfiguration)

Presents an edit menu using the object you provide for configuration.

func reloadVisibleMenu()

Updates the actions an edit menu displays.

func updateVisibleMenuPosition(animated: Bool)

Updates the position of the currently visible menu with an option to animate the action.

func dismissMenu()

Dismiss the edit menu if present.

func location(in: UIView?) -> CGPoint

Returns the location of the user interaction in the specified view’s coordinate system.

