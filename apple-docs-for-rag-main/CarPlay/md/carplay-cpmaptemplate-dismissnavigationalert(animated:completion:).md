

- CarPlay
- CPMapTemplate
-  dismissNavigationAlert(animated:completion:) 

Instance Method

# dismissNavigationAlert(animated:completion:)

Tells the map template to dismiss the visable navigation alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func dismissNavigationAlert(
    animated: Bool,
    completion: @escaping (Bool) -> Void
)
```

``` source
func dismissNavigationAlert(animated: Bool) async -> Bool
```

## Parameters 

`animated`  

Determines whether the system should animate the dismissal of the navigation alert. Set to true to animate the dismissal.

`completion`  

The block invoked after dismissing the navigation alert. The Bool argument in the block indicates whether the template dismissed an alert.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func dismissNavigationAlert(animated: Bool) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Displaying a Navigation Alert

func present(navigationAlert: CPNavigationAlert, animated: Bool)

Displays a navigation alert on the map template.

var currentNavigationAlert: CPNavigationAlert?

The visible navigation alert.

class CPNavigationAlert

An alert that displays map- or navigation-related information to the user.

