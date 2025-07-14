

- Exposure Notification
- ENManager
-  setExposureNotificationEnabled(\_:completionHandler:) 

Instance Method

# setExposureNotificationEnabled(\_:completionHandler:)

Enables or disables exposure notification.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
func setExposureNotificationEnabled(
    _ enabled: Bool,
    completionHandler: @escaping ENErrorHandler
)
```

``` source
func setExposureNotificationEnabled(_ enabled: Bool) async throws
```

## Parameters 

`enabled`  

A Boolean that enables or disables exposure notification.

`completionHandler`  

The completion handler that the framework calls once exposure notification is enabled or disabled.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setExposureNotificationEnabled(_ enabled: Bool) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Important

This method is available in iOS 12.5, and in iOS 13.5 and later.

If the user hasn’t authorized exposure notification, this method displays a user dialog requesting consent.

Note

Using this method to disable exposure notification stops scanning and Bluetooth advertising, but diagnosis keys and data remain.

## See Also

### Activating the Manager

func activate(completionHandler: ENErrorHandler)

Prepares the manager for use.

var activityHandler: ENActivityHandler?

The handler that the framework invokes when the app activates a notification manager.

typealias ENActivityHandler

The handler the system invokes to report activities that occurred while the app wasn’t running.

struct ENActivityFlags

Activities that occur while the app isn’t running.

