

- UIKit
- UIActivity
-  activityType 

Instance Property

# activityType

The type of service being provided.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var activityType: UIActivity.ActivityType? { get }
```

## Discussion

The default value is `nil`. Subclasses may override this property to return a custom activity type that’s reported to the completionWithItemsHandler completion handler.

## See Also

### Getting the activity information

class var activityCategory: UIActivity.Category

The category of the activity, which may be used to group activities in the UI.

enum Category

An enumeration that defines categories of activities.

struct ActivityType

A structure that describes the types of activities for which the system has built-in support.

var activityTitle: String?

A user-readable string that describes the service.

var activityImage: UIImage?

An image that identifies the service to the user.

