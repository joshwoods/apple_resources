

- UIKit
- UIActivity
-  activityTitle 

Instance Property

# activityTitle

A user-readable string that describes the service.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var activityTitle: String? { get }
```

## Return Value

A string that describes the service.

## Discussion

The default value is `nil`. Subclasses must override this property to return a user-readable string that describes the service. The string you return should be localized.

## See Also

### Getting the activity information

class var activityCategory: UIActivity.Category

The category of the activity, which may be used to group activities in the UI.

enum Category

An enumeration that defines categories of activities.

var activityType: UIActivity.ActivityType?

The type of service being provided.

struct ActivityType

A structure that describes the types of activities for which the system has built-in support.

var activityImage: UIImage?

An image that identifies the service to the user.

