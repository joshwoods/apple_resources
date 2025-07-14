

- Exposure Notification
-  ENExposureDaySummary 

Class

# ENExposureDaySummary

The summary of exposure information for a single day.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
class ENExposureDaySummary
```

## Overview

Important

This class is available in iOS 12.5, and in iOS 13.7 and later.

## Topics

### Getting Exposure Summary Information

var date: Date

The date that the exposure occurred.

var confirmedClinicalDiagnosisSummary: ENExposureSummaryItem?

The summary of exposures from a clinically-originated diagnosis.

var confirmedTestSummary: ENExposureSummaryItem?

The summary of exposures with a confirmed diagnosis.

var recursiveSummary: ENExposureSummaryItem?

The summary of exposures that came from someone else who was exposed.

var selfReportedSummary: ENExposureSummaryItem?

The summary of self-reported exposures.

var daySummary: ENExposureSummaryItem

The summary of all exposures for the day.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Summaries

class ENExposureDetectionSummary

A summary of exposures.

class ENExposureSummaryItem

The summary of exposures for a specific time period or report type.

