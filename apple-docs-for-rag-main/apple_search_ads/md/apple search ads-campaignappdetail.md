

- Apple Search Ads
-  CampaignAppDetail 

Object

# CampaignAppDetail

The app data to fetch from campaign-level reports.

Search Ads 2.0+

``` source
object CampaignAppDetail
```

## Properties

`adamId`

`int64`

Displays as `app:{adamId}` in ReportingCampaign.

Each time you use an `adamId` in the API, it must match the `adamId` in your campaign. Use Get a Campaign or Get all Campaigns to obtain your `adamId` and correlate it to the correct campaign.

`appName`

`string`

The App Store Connect app identifier, which displays as `app:{appName}` in ReportingCampaign.

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

object InsightsObject

The container object for bid recommendations.

object KeywordInsights

The object that contains bid recommendations.

