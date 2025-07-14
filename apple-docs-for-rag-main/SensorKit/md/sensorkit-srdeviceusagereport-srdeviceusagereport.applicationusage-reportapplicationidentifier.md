

- SensorKit
- SRDeviceUsageReport
- SRDeviceUsageReport.ApplicationUsage
-  reportApplicationIdentifier 

Instance Property

# reportApplicationIdentifier

A pseudonymn for a real application identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var reportApplicationIdentifier: String { get }
```

## Discussion

The value of this property uniquely refers to a single app throughout the report without revealing the app’s true identity. For user privacy, the system assigns this property a pseudonymous string in cases where the bundleIdentifier is `nil`.

## See Also

### Identifying the App

var bundleIdentifier: String?

The bundle identifier of the app in use.

var supplementalCategories: [SRSupplementalCategory]

Categories that provide more information about an app.

class SRSupplementalCategory

A more detailed category that provides additional context to the app category.

