

- Exposure Notification
- ENExposureDaySummary
-  confirmedClinicalDiagnosisSummary 

Instance Property

# confirmedClinicalDiagnosisSummary

The summary of exposures from a clinically-originated diagnosis.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var confirmedClinicalDiagnosisSummary: ENExposureSummaryItem? { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

## See Also

### Getting Exposure Summary Information

var date: Date

The date that the exposure occurred.

var confirmedTestSummary: ENExposureSummaryItem?

The summary of exposures with a confirmed diagnosis.

var recursiveSummary: ENExposureSummaryItem?

The summary of exposures that came from someone else who was exposed.

var selfReportedSummary: ENExposureSummaryItem?

The summary of self-reported exposures.

var daySummary: ENExposureSummaryItem

The summary of all exposures for the day.

