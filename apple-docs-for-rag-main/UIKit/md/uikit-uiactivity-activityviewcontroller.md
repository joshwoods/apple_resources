

- UIKit
- UIActivity
-  activityViewController 

Instance Property

# activityViewController

The view controller to present to the user.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var activityViewController: UIViewController? { get }
```

## Discussion

Subclasses that provide additional UI using a view controller can override this method to return that view controller. If this method returns a valid object, the system presents the returned view controller modally instead of calling the perform() method.

Your custom view controller should provide a view with your custom UI and should handle any user interactions inside those views. Upon completing the activity, don’t dismiss the view controller yourself. Instead, call the activityDidFinish(_:) method and let the system dismiss it for you.

## See Also

### Performing the activity

func canPerform(withActivityItems: [Any]) -> Bool

Queries whether the service can act on the specified data items.

func prepare(withActivityItems: [Any])

Prepares your service to act on the specified data.

func perform()

Performs the service when no custom view controller is provided.

func activityDidFinish(Bool)

Notifies the system that your activity object has completed its work.

