

- UIKit
- UIActivityViewController
-  UIActivityViewController.CompletionHandler Deprecated

Type Alias

# UIActivityViewController.CompletionHandler

A completion handler to execute after the activity view controller is dismissed.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
typealias CompletionHandler = (UIActivity.ActivityType?, Bool) -> Void
```

Deprecated

Use UIActivityViewController.CompletionWithItemsHandler instead.

## Discussion

Upon the completion of an activity, or the dismissal of the activity view controller, the view controller’s completion block is executed. You can use this block to execute any final code related to the service. The parameters of this block are as follows:

activityType  
The type of the service that was selected by the user. For custom services, this is the value returned by the activityType method of a UIActivity object. For system-defined activities, it is one of the strings listed in “Built-in Activity Types” in UIActivity.

completed  
true if the service was performed or false if it was not. This parameter is also set to false when the user dismisses the view controller without selecting a service.

## See Also

### Deprecated

var completionHandler: UIActivityViewController.CompletionHandler?

The completion handler to execute after the activity view controller is dismissed.

Deprecated

