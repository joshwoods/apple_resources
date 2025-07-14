

- Exposure Notification
- ENExposureDaySummary
-  selfReportedSummary 

Instance Property

# selfReportedSummary

The summary of self-reported exposures.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var selfReportedSummary: ENExposureSummaryItem? { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

## See Also

### Getting Exposure Summary Information

var date: Date

The date that the exposure occurred.

var confirmedClinicalDiagnosisSummary: ENExposureSummaryItem?

The summary of exposures from a clinically-originated diagnosis.

var confirmedTestSummary: ENExposureSummaryItem?

The summary of exposures with a confirmed diagnosis.

var recursiveSummary: ENExposureSummaryItem?

The summary of exposures that came from someone else who was exposed.

var daySummary: ENExposureSummaryItem

The summary of all exposures for the day.

