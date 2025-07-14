

- UIKit
- UIEditMenuInteraction
-  location(in:) 

Instance Method

# location(in:)

Returns the location of the user interaction in the specified view’s coordinate system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func location(in view: UIView?) -> CGPoint
```

## Parameters 

`view`  

The view containing the target coordinate system. To return a point in the window’s coordinate system, specify `nil`.

## Return Value

The location of the interaction in the coordinate system of view.

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

func dismissMenu()

Dismiss the edit menu if present.

