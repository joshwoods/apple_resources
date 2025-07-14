

- UIKit
- UIActivity
-  activityDidFinish(\_:) 

Instance Method

# activityDidFinish(\_:)

Notifies the system that your activity object has completed its work.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func activityDidFinish(_ completed: Bool)
```

## Parameters 

`completed`  

Specify true if the service executed to completion or false if the service was canceled or didn’t finish because of an error.

## Discussion

This method dismisses the sharing interface provided by the UIActivityViewController object. If you provided a view controller using the activityViewController method, this method dismisses that view controller too.

You must call this method after completing the work associated with this object’s service. This is true regardless of whether you used the activityViewController or perform() method to initiate the service. When calling the method, use the Boolean value to indicate whether the service completed successfully.

This method must be called on the main thread.

## See Also

### Performing the activity

func canPerform(withActivityItems: [Any]) -> Bool

Queries whether the service can act on the specified data items.

func prepare(withActivityItems: [Any])

Prepares your service to act on the specified data.

var activityViewController: UIViewController?

The view controller to present to the user.

func perform()

Performs the service when no custom view controller is provided.

