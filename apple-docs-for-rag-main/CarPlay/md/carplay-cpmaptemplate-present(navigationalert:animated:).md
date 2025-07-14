

- CarPlay
- CPMapTemplate
-  present(navigationAlert:animated:) 

Instance Method

# present(navigationAlert:animated:)

Displays a navigation alert on the map template.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func present(
    navigationAlert: CPNavigationAlert,
    animated: Bool
)
```

## Parameters 

`navigationAlert`  

The navigation alert to display.

`animated`  

To animate the display of the alert, set to true; otherwise, set to false to immediately display the alert.

## Discussion

This method has no effect when the map template is already displaying a navigation alert. Dismiss the current alert before presenting a new one.

## See Also

### Displaying a Navigation Alert

func dismissNavigationAlert(animated: Bool, completion: (Bool) -> Void)

Tells the map template to dismiss the visable navigation alert.

var currentNavigationAlert: CPNavigationAlert?

The visible navigation alert.

class CPNavigationAlert

An alert that displays map- or navigation-related information to the user.

