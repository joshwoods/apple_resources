

- Exposure Notification
-  ENActivityHandler 

Type Alias

# ENActivityHandler

The handler the system invokes to report activities that occurred while the app wasn’t running.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
typealias ENActivityHandler = (ENActivityFlags) -> Void
```

## Parameters 

`activityFlags`  

The flags indicating what activity occured while the app wasn’t running.

## See Also

### Activating the Manager

func activate(completionHandler: ENErrorHandler)

Prepares the manager for use.

var activityHandler: ENActivityHandler?

The handler that the framework invokes when the app activates a notification manager.

struct ENActivityFlags

Activities that occur while the app isn’t running.

func setExposureNotificationEnabled(Bool, completionHandler: ENErrorHandler)

Enables or disables exposure notification.

