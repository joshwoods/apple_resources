

- HealthKit
- HKSampleType
-  minimumAllowedDuration 

Instance Property

# minimumAllowedDuration

The minimum duration if the sample type has a restricted duration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var minimumAllowedDuration: TimeInterval { get }
```

## Return Value

The minimum time interval between the sample’s startDate and endDate properties.

## Discussion

This method throws an exception if isMinimumDurationRestricted is false.

## See Also

### Checking the Duration Restriction

var isMinimumDurationRestricted: Bool

A Boolean value that indicates whether samples of this type have a minimum time interval between the start and end dates.

var isMaximumDurationRestricted: Bool

A Boolean value that indicates whether samples of this type have a maximum time interval between the start and end dates.

var maximumAllowedDuration: TimeInterval

The maximum duration if the sample type has a restricted duration.

