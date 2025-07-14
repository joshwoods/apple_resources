

- Exposure Notification
- ENManager
-  activityHandler 

Instance Property

# activityHandler

The handler that the framework invokes when the app activates a notification manager.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var activityHandler: ENActivityHandler? { get set }
```

## Discussion

When the app launches, it creates an ENManager instance, sets this handler, and then activates the manager.

## See Also

### Activating the Manager

func activate(completionHandler: ENErrorHandler)

Prepares the manager for use.

typealias ENActivityHandler

The handler the system invokes to report activities that occurred while the app wasn’t running.

struct ENActivityFlags

Activities that occur while the app isn’t running.

func setExposureNotificationEnabled(Bool, completionHandler: ENErrorHandler)

Enables or disables exposure notification.

