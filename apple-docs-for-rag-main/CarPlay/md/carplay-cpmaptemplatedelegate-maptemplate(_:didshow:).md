

- CarPlay
- CPMapTemplateDelegate
-  mapTemplate(\_:didShow:) 

Instance Method

# mapTemplate(\_:didShow:)

Tells the delegate that the system showed the navigation alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func mapTemplate(
    _ mapTemplate: CPMapTemplate,
    didShow navigationAlert: CPNavigationAlert
)
```

## Parameters 

`mapTemplate`  

The current map template.

`navigationAlert`  

The navigation alert presented by the system.

## See Also

### Handling Navigation Alerts

func mapTemplate(CPMapTemplate, willShow: CPNavigationAlert)

Tells the delegate that the system will show the navigation alert.

func mapTemplate(CPMapTemplate, willDismiss: CPNavigationAlert, dismissalContext: CPNavigationAlert.DismissalContext)

Tells the delegate that the system is preparing to dismiss the navigation alert.

func mapTemplate(CPMapTemplate, didDismiss: CPNavigationAlert, dismissalContext: CPNavigationAlert.DismissalContext)

Tells the delegate that the system dismissed the navigation alert.

enum DismissalContext

A set of reasons for dismissing a navigation alert.

