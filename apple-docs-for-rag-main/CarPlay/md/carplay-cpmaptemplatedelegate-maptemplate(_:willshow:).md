

- CarPlay
- CPMapTemplateDelegate
-  mapTemplate(\_:willShow:) 

Instance Method

# mapTemplate(\_:willShow:)

Tells the delegate that the system will show the navigation alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func mapTemplate(
    _ mapTemplate: CPMapTemplate,
    willShow navigationAlert: CPNavigationAlert
)
```

## Parameters 

`mapTemplate`  

The current map template.

`navigationAlert`  

The navigation alert to display.

## See Also

### Handling Navigation Alerts

func mapTemplate(CPMapTemplate, didShow: CPNavigationAlert)

Tells the delegate that the system showed the navigation alert.

func mapTemplate(CPMapTemplate, willDismiss: CPNavigationAlert, dismissalContext: CPNavigationAlert.DismissalContext)

Tells the delegate that the system is preparing to dismiss the navigation alert.

func mapTemplate(CPMapTemplate, didDismiss: CPNavigationAlert, dismissalContext: CPNavigationAlert.DismissalContext)

Tells the delegate that the system dismissed the navigation alert.

enum DismissalContext

A set of reasons for dismissing a navigation alert.

