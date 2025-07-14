

- UIKit
- UIAlertController
-  actions 

Instance Property

# actions

The actions that the user can take in response to the alert or action sheet.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var actions: [UIAlertAction] { get }
```

## Discussion

The actions are in the order in which you added them to the alert controller. This order also corresponds to the order in which they’re displayed in the alert or action sheet. The second action in the array is displayed below the first, the third is displayed below the second, and so on.

## See Also

### Configuring the user actions

func addAction(UIAlertAction)

Attaches an action object to the alert or action sheet.

var preferredAction: UIAlertAction?

The preferred action for the user to take from an alert.

