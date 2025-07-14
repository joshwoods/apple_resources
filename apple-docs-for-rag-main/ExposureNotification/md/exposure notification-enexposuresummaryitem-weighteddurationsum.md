

- Exposure Notification
- ENExposureSummaryItem
-  weightedDurationSum 

Instance Property

# weightedDurationSum

The sum of exposure durations weighted by their attenuation.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var weightedDurationSum: TimeInterval { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

This value is stored as seconds, rounded up to the next minute. Divide by 60 to convert to minutes when displaying to the user.

weightedDurationSum ignores infectiousness and diagnosisReportType; therefore, it can be nonzero for encounters that have a infectiousness weight or diagnosis report type weight of `0`.

## See Also

### Getting Summary Properties

var maximumScore: Double

The highest score of all exposures for this item.

var scoreSum: Double

The sum of scores for all exposure for this item.

