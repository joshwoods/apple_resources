

- UIKit
- UIAccessibility
-  post(notification:argument:) 

Type Method

# post(notification:argument:)

Posts a notification to assistive apps.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
static func post(
    notification: UIAccessibility.Notification,
    argument: Any?
)
```

## Parameters 

`notification`  

The notification to post (see “Notifications” in UIAccessibility for a list of notifications).

`argument`  

The argument specified by the notification. Pass `nil` unless a notification specifies otherwise.

## Discussion

Your application might need to post accessibility notifications if you have user interface components that change very frequently or that appear and disappear.

## See Also

### Notifications

Notification names

The names of notifications that the accessibility system generates.

Notification dictionary keys

Handle notifications with keys in the user info dictionary.

