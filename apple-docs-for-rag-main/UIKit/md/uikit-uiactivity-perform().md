

- UIKit
- UIActivity
-  perform() 

Instance Method

# perform()

Performs the service when no custom view controller is provided.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func perform()
```

## Discussion

The default implementation of this method does nothing. If your service doesn’t provide any custom UI using the activityViewController method, override this method and use it to perform the activity. Your activity must operate on the data items received in the prepare(withActivityItems:) method.

This method is called on your app’s main thread. If your app can complete the activity quickly on the main thread, do so and call the activityDidFinish(_:) method when it’s done. If performing the activity might take some time, use this method to start the work in the background and then exit without calling activityDidFinish(_:) from this method. When your background work has completed, call activityDidFinish(_:). You must call activityDidFinish(_:) on the main thread.

## See Also

### Performing the activity

func canPerform(withActivityItems: [Any]) -> Bool

Queries whether the service can act on the specified data items.

func prepare(withActivityItems: [Any])

Prepares your service to act on the specified data.

var activityViewController: UIViewController?

The view controller to present to the user.

func activityDidFinish(Bool)

Notifies the system that your activity object has completed its work.

