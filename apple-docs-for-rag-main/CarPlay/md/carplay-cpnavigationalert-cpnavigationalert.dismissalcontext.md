

- CarPlay
- CPNavigationAlert
-  CPNavigationAlert.DismissalContext 

Enumeration

# CPNavigationAlert.DismissalContext

A set of reasons for dismissing a navigation alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
enum DismissalContext
```

## Topics

### Dismissal Reasons

case timeout

The system dismissed the navigation alert due to a timeout.

case systemDismissed

The system dismissed the navigation alert.

case userDismissed

The user dismissed the navigation alert.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling Navigation Alerts

func mapTemplate(CPMapTemplate, willShow: CPNavigationAlert)

Tells the delegate that the system will show the navigation alert.

func mapTemplate(CPMapTemplate, didShow: CPNavigationAlert)

Tells the delegate that the system showed the navigation alert.

func mapTemplate(CPMapTemplate, willDismiss: CPNavigationAlert, dismissalContext: CPNavigationAlert.DismissalContext)

Tells the delegate that the system is preparing to dismiss the navigation alert.

func mapTemplate(CPMapTemplate, didDismiss: CPNavigationAlert, dismissalContext: CPNavigationAlert.DismissalContext)

Tells the delegate that the system dismissed the navigation alert.

