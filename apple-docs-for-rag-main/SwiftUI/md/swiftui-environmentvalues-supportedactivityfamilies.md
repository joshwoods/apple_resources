

- SwiftUI
- EnvironmentValues
-  supportedActivityFamilies 

Instance Property

# supportedActivityFamilies

An environment value that that indicates potential rendered family for a Live Activity.

iOS 18.0+iPadOS 18.0+

``` source
var supportedActivityFamilies: Set { get set }
```

## Discussion

To detect the currently rendered activity family size, use the activityFamily environment variable. The `supportedActivityFamilies` environment value might only be useful if your make you make your Live Activity views available in a Swift package.

