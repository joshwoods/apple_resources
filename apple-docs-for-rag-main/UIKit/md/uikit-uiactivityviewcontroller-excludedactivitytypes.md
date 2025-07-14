

- UIKit
- UIActivityViewController
-  excludedActivityTypes 

Instance Property

# excludedActivityTypes

The list of services that should not be displayed.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var excludedActivityTypes: [UIActivity.ActivityType]? { get set }
```

## Discussion

This property contains an array of strings, each of which corresponds to the value you would find in the activityType parameter of a UIActivity object. Each string you specify indicates a service that you do not want displayed to the user. You might exclude services that you feel are not suitable for the content you are providing. For example, you might not want to allow the user to print a specific image. If the value of this property is `nil`, no services are excluded.

This value of this property is `nil` by default.

