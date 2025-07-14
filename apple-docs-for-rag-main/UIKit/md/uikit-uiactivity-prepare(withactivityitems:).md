

- UIKit
- UIActivity
-  prepare(withActivityItems:) 

Instance Method

# prepare(withActivityItems:)

Prepares your service to act on the specified data.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func prepare(withActivityItems activityItems: [Any])
```

## Parameters 

`activityItems`  

An array of objects of varying types. These are the data objects on which to act.

## Discussion

The default implementation of this method does nothing. This method is called after the user has selected your service but before your service is asked to perform its action. Subclasses should override this method and use it to store a reference to the data items in the `activityItems` parameter. In addition, if the implementation of your service requires displaying additional UI to the user, you can use this method to prepare your view controller object and make it available from the activityViewController method.

## See Also

### Performing the activity

func canPerform(withActivityItems: [Any]) -> Bool

Queries whether the service can act on the specified data items.

var activityViewController: UIViewController?

The view controller to present to the user.

func perform()

Performs the service when no custom view controller is provided.

func activityDidFinish(Bool)

Notifies the system that your activity object has completed its work.

