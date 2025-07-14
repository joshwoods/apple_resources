

- Foundation
- NSUserActivity
-  isEligibleForHandoff 

Instance Property

# isEligibleForHandoff

A Boolean value that indicates whether the activity can be continued on another device using Handoff.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var isEligibleForHandoff: Bool { get set }
```

## Mentioned in 

Creating a user activity object

## Discussion

The default value of this property is true.

## See Also

### Specifying the activity’s eligibility

var isEligibleForSearch: Bool

A Boolean value that indicates whether the activity should be added to the on-device index.

var isEligibleForPublicIndexing: Bool

A Boolean value that indicates whether the activity can be publicly accessed by all iOS users.

var expirationDate: Date?

The date after which the activity is no longer eligible for Handoff or indexing.

