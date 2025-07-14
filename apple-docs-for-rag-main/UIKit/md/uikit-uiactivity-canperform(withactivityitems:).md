

- UIKit
- UIActivity
-  canPerform(withActivityItems:) 

Instance Method

# canPerform(withActivityItems:)

Queries whether the service can act on the specified data items.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func canPerform(withActivityItems activityItems: [Any]) -> Bool
```

## Parameters 

`activityItems`  

An array of objects of varying types. These are the data objects on which the service would act.

## Return Value

true if your service can act on the specified data items or false if it cannot.

## Discussion

The default implementation of this method returns false. Subclasses must override it and return true if the data in the `activityItems` parameter can be operated on by your service. Your implementation should check the types of the objects in the array and use that information to determine if your service can act on the corresponding data.

The UIActivityViewController object calls this method when determining which services to show to the user.

## See Also

### Performing the activity

func prepare(withActivityItems: [Any])

Prepares your service to act on the specified data.

var activityViewController: UIViewController?

The view controller to present to the user.

func perform()

Performs the service when no custom view controller is provided.

func activityDidFinish(Bool)

Notifies the system that your activity object has completed its work.

