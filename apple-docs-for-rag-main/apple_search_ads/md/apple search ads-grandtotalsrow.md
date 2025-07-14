

- Apple Search Ads
-  GrandTotalsRow 

Object

# GrandTotalsRow

The summary of cumulative metrics.

Search Ads 2.0+

``` source
object GrandTotalsRow
```

## Properties

`other`

`boolean`

The impressions that return in reports when there are fewer than 100 demographic dimensions, and fewer than 10 search terms. If `Other` is `true`, the corresponding dimensions are `null`.

`total`

SpendRow

The tap, conversion, and monetary totals (SpendRow) in the response. This is the same as ExtendedSpendRow except it doesn’t include the `date` attribute.

## See Also

### Reports Request and Response Objects

object ReportingRequest

The report request body.

object ReportingResponseBody

The container object for the report response body.

object ReportingResponse

The container object of report metrics.

object ReportingDataResponse

The total metrics for a report.

object SpendRow

The reporting response metrics.

object ExtendedSpendRow

The descriptions of metrics with dates.

object Row

The report metrics by time granularity.

object ReportingCampaign

The response to a request to fetch campaign-level reports.

object ReportingAdGroup

The response to a request to fetch ad group-level reports.

object ReportingKeyword

The response to a request to fetch keyword-level reports.

object ReportingSearchTerm

The response to a request to fetch search term-level reports.

object ReportingAd

The response to a request to fetch ad-level reports.

object CampaignAppDetail

The app data to fetch from campaign-level reports.

object InsightsObject

The container object for bid recommendations.

object KeywordInsights

The object that contains bid recommendations.

