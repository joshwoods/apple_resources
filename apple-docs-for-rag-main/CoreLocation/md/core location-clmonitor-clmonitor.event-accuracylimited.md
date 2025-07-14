

- Core Location
- CLMonitor
- CLMonitor.Event
-  accuracyLimited 

Instance Property

# accuracyLimited

A Boolean value that indicates whether the app receives accuracy-limited location updates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var accuracyLimited: Bool { get }
```

## Discussion

If this property is true, then the app receives accuracy-limited location updates.

## See Also

### Event states

var authorizationDenied: Bool

A Boolean value that indicates whether the app has local authorization.

var authorizationDeniedGlobally: Bool

A Boolean value that indicates whether the app has system-wide authorization.

var authorizationRequestInProgress: Bool

var authorizationRestricted: Bool

A Boolean value that indicates whether the app can make authorization changes.

var conditionLimitExceeded: Bool

A Boolean value that indicates whether the app receives location updates based on other monitoring conditions.

var conditionUnsupported: Bool

A Boolean value that indicates whether the app receives location updates based on the supported condition.

var insufficientlyInUse: Bool

A Boolean value that indicates whether the app receives location updates because it’s insufficiently in use.

var persistenceUnavailable: Bool

A Boolean value that indicates whether it receives location updates based on successful persistence.

var serviceSessionRequired: Bool

