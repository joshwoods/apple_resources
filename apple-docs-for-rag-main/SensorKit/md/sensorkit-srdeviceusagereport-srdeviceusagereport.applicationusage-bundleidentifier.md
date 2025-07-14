

- SensorKit
- SRDeviceUsageReport
- SRDeviceUsageReport.ApplicationUsage
-  bundleIdentifier 

Instance Property

# bundleIdentifier

The bundle identifier of the app in use.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var bundleIdentifier: String? { get }
```

## Discussion

The framework sets a value for this property only if the bundle identifier corresponds to an Apple app. Otherwise, you can correlate the app by using the reportApplicationIdentifier property.

## See Also

### Identifying the App

var reportApplicationIdentifier: String

A pseudonymn for a real application identifier.

var supplementalCategories: [SRSupplementalCategory]

Categories that provide more information about an app.

class SRSupplementalCategory

A more detailed category that provides additional context to the app category.

