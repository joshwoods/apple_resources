

- CarPlay
- CPMapTemplateDelegate
-  mapTemplate(\_:willDismiss:dismissalContext:) 

Instance Method

# mapTemplate(\_:willDismiss:dismissalContext:)

Tells the delegate that the system is preparing to dismiss the navigation alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func mapTemplate(
    _ mapTemplate: CPMapTemplate,
    willDismiss navigationAlert: CPNavigationAlert,
    dismissalContext: CPNavigationAlert.DismissalContext
)
```

## Parameters 

`mapTemplate`  

The current map template.

`navigationAlert`  

The navigation alert to dismiss.

`dismissalContext`  

The reason for dismissing the navigation alert.

## See Also

### Handling Navigation Alerts

func mapTemplate(CPMapTemplate, willShow: CPNavigationAlert)

Tells the delegate that the system will show the navigation alert.

func mapTemplate(CPMapTemplate, didShow: CPNavigationAlert)

Tells the delegate that the system showed the navigation alert.

func mapTemplate(CPMapTemplate, didDismiss: CPNavigationAlert, dismissalContext: CPNavigationAlert.DismissalContext)

Tells the delegate that the system dismissed the navigation alert.

enum DismissalContext

A set of reasons for dismissing a navigation alert.

