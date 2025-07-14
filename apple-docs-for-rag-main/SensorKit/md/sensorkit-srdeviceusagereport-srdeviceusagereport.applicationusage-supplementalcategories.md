

- SensorKit
- SRDeviceUsageReport
- SRDeviceUsageReport.ApplicationUsage
-  supplementalCategories 

Instance Property

# supplementalCategories

Categories that provide more information about an app.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
var supplementalCategories: [SRSupplementalCategory] { get }
```

## See Also

### Identifying the App

var bundleIdentifier: String?

The bundle identifier of the app in use.

var reportApplicationIdentifier: String

A pseudonymn for a real application identifier.

class SRSupplementalCategory

A more detailed category that provides additional context to the app category.

