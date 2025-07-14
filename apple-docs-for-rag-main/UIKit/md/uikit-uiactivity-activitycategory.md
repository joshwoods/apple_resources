

- UIKit
- UIActivity
-  activityCategory 

Type Property

# activityCategory

The category of the activity, which may be used to group activities in the UI.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class var activityCategory: UIActivity.Category { get }
```

## Return Value

The assigned category of the activity. The default implementation returns UIActivity.Category.action.

## Discussion

Override this property to define a different activity category for your custom activity.

## See Also

### Getting the activity information

enum Category

An enumeration that defines categories of activities.

var activityType: UIActivity.ActivityType?

The type of service being provided.

struct ActivityType

A structure that describes the types of activities for which the system has built-in support.

var activityTitle: String?

A user-readable string that describes the service.

var activityImage: UIImage?

An image that identifies the service to the user.

