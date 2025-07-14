

- CarPlay
- CPMapTemplate
-  currentNavigationAlert 

Instance Property

# currentNavigationAlert

The visible navigation alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var currentNavigationAlert: CPNavigationAlert? { get }
```

## Discussion

If a navigation alert isn’t visible, the property returns nil.

## See Also

### Displaying a Navigation Alert

func present(navigationAlert: CPNavigationAlert, animated: Bool)

Displays a navigation alert on the map template.

func dismissNavigationAlert(animated: Bool, completion: (Bool) -> Void)

Tells the map template to dismiss the visable navigation alert.

class CPNavigationAlert

An alert that displays map- or navigation-related information to the user.

