

- Apple Search Ads
-  KeywordBidRecommendation 

Object

# KeywordBidRecommendation

The suggested bid amount for a keyword.

Search Ads 3.0+

``` source
object KeywordBidRecommendation
```

## Properties

`suggestedBidAmount`

Money

An indicator that varies over time to help you incrementally increase the likelihood of your ad showing in searches in the App Store. A `suggestedBidAmount` isn’t a representation of a bid floor or ceiling. A `suggestedBidAmount` is based on various factors, including, but not limited to, historical data related to past performance and recommendations. Actual outcomes, including changes in spend and average CPA, may vary.

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

In Apple Search Ads Campaign Management API 5, the `suggestedBidAmount` field replaces the deprecated `bidMin` and `bidMax` fields.

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

object GrandTotalsRow

The summary of cumulative metrics.

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

