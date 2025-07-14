

- UIKit
- UIAlertController
-  preferredAction 

Instance Property

# preferredAction

The preferred action for the user to take from an alert.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var preferredAction: UIAlertAction? { get set }
```

## Discussion

The preferred action is relevant for the UIAlertController.Style.alert style only; it isn’t used by action sheets. When you specify a preferred action, the alert controller highlights the text of that action to give it emphasis. (If the alert also contains a cancel button, the preferred action receives the highlighting instead of the cancel button.) If the iOS device is connected to a physical keyboard, pressing the Return key triggers the preferred action.

The action object you assign to this property must have already been added to the alert controller’s list of actions. Assigning an object to this property before adding it with the addAction(_:) method is a programmer error.

The default value of this property is `nil`.

## See Also

### Configuring the user actions

func addAction(UIAlertAction)

Attaches an action object to the alert or action sheet.

var actions: [UIAlertAction]

The actions that the user can take in response to the alert or action sheet.

