

- MetricKit
- MXLocationActivityMetric
-  cumulativeBestAccuracyForNavigationTime 

Instance Property

# cumulativeBestAccuracyForNavigationTime

The total time spent tracking the current location at the best accuracy for navigation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var cumulativeBestAccuracyForNavigationTime: Measurement { get }
```

## See Also

### Reading location services use

var cumulativeBestAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location at the best accuracy.

var cumulativeNearestTenMetersAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location to an accuracy of 10 meters.

var cumulativeHundredMetersAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location to an accuracy of 100 meters.

var cumulativeKilometerAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location to an accuracy of 1 kilometer.

var cumulativeThreeKilometersAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location to an accuracy of 3 kilometers.

