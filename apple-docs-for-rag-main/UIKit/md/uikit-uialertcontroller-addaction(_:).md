

- UIKit
- UIAlertController
-  addAction(\_:) 

Instance Method

# addAction(\_:)

Attaches an action object to the alert or action sheet.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addAction(_ action: UIAlertAction)
```

## Parameters 

`action`  

The action object to display as part of the alert. Actions are displayed as buttons in the alert. The action object provides the button text and the action to be performed when that button is tapped.

## Discussion

If your alert has multiple actions, the order in which you add those actions determines their order in the resulting alert or action sheet.

## See Also

### Configuring the user actions

var actions: [UIAlertAction]

The actions that the user can take in response to the alert or action sheet.

var preferredAction: UIAlertAction?

The preferred action for the user to take from an alert.

