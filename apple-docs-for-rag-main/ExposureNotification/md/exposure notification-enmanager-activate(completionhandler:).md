

- Exposure Notification
- ENManager
-  activate(completionHandler:) 

Instance Method

# activate(completionHandler:)

Prepares the manager for use.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
func activate(completionHandler: @escaping ENErrorHandler)
```

``` source
func activate() async throws
```

## Parameters 

`completionHandler`  

The completion handler that the framework calls when activation completes.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func activate() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Important

This method is available in iOS 12.5, and in iOS 13.5 and later.

Properties may not be usable until the completion handler reports success.

## See Also

### Activating the Manager

var activityHandler: ENActivityHandler?

The handler that the framework invokes when the app activates a notification manager.

typealias ENActivityHandler

The handler the system invokes to report activities that occurred while the app wasn’t running.

struct ENActivityFlags

Activities that occur while the app isn’t running.

func setExposureNotificationEnabled(Bool, completionHandler: ENErrorHandler)

Enables or disables exposure notification.

