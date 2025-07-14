

- Core Location
- CLMonitor
- CLMonitor.Event
-  insufficientlyInUse 

Instance Property

# insufficientlyInUse

A Boolean value that indicates whether the app receives location updates because it’s insufficiently in use.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var insufficientlyInUse: Bool { get }
```

## Discussion

If this property is true, then the app isn’t receiving location updates because it’s insufficiently in use.

## See Also

### Event states

var accuracyLimited: Bool

A Boolean value that indicates whether the app receives accuracy-limited location updates.

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

var persistenceUnavailable: Bool

A Boolean value that indicates whether it receives location updates based on successful persistence.

var serviceSessionRequired: Bool

