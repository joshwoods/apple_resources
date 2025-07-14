

- HealthKit
- HKSampleType
-  isMinimumDurationRestricted 

Instance Property

# isMinimumDurationRestricted

A Boolean value that indicates whether samples of this type have a minimum time interval between the start and end dates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isMinimumDurationRestricted: Bool { get }
```

## See Also

### Checking the Duration Restriction

var minimumAllowedDuration: TimeInterval

The minimum duration if the sample type has a restricted duration.

var isMaximumDurationRestricted: Bool

A Boolean value that indicates whether samples of this type have a maximum time interval between the start and end dates.

var maximumAllowedDuration: TimeInterval

The maximum duration if the sample type has a restricted duration.

