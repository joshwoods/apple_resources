

- Apple Search Ads
-  SpendRow 

Object

# SpendRow

The reporting response metrics.

Search Ads 2.0+

``` source
object SpendRow
```

## Properties

`avgCPM`

Money

The average CPM is the average amount you pay per one thousand ad impressions.

`avgCPT`

Money

The average cost-per-tap (CPT) is the ratio of spend over taps.

`impressions`

`int64`

The number of times your ad appears in App Store search results within the reporting period.

`localSpend`

Money

The total spend of a campaign in the currency the organization uses.

`tapInstallCPI`

Money

Prior to API 5, this was the `avgCPA` field.

The total campaign spend divided by the number of tap-through installs within the reporting period.

`tapInstallRate`

`double`

Prior to API 5, this was the `conversionRate` field.

The total number of tap-through installs divided by the total number of taps within the reporting period.

`tapInstalls`

`int64`

Prior to API 5, this was the `installs` field.

The total number of new downloads and redownloads from people who tapped your ad within a 30-day attribution window.

`tapNewDownloads`

`int64`

Prior to API 5, this was the `newDownloads` field.

New downloads from people who tapped your ad within a 30-day attribution window.

The API counts new downloads when someone downloads your app to a device where your app hasn’t previously been installed.

`tapRedownloads`

`int64`

Prior to API 5, this was the `redownloads` field.

Redownloads from people who tapped your ad within a 30-day attribution window.

The API counts redownloads when someone downloads your app, deletes it, and downloads it again on the same device, or a different one, following an ad tap.

`taps`

`int64`

The number of times people tap your ad within the reporting period.

`totalAvgCPI`

Money

The total campaign spend divided by the total number of installs within the reporting period.

`totalInstallRate`

`double`

The total number of installs divided by the total number of taps within the reporting period.

`totalInstalls`

`int64`

The total number of tap-through and view-through new downloads and redownloads within the reporting period.

`totalNewDownloads`

`int64`

The total number of tap-through and view-through new downloads within the reporting period.

`totalRedownloads`

`int64`

The total number of tap-through and view-through redownloads within the reporting period.

`ttr`

`double`

The tap-through rate (TTR) is the number of times people tap your ad divided by the total impressions your ad receives.

`viewInstalls`

`int64`

The total number of new downloads and redownloads from people who viewed your ad, but didn’t tap it, within a 1-day attribution window.

`viewNewDownloads`

`int64`

New downloads from people who viewed your ad, but didn’t tap it, within a 1-day attribution window. The API counts new downloads when someone downloads your app to a device where your app hasn’t previously been installed.

`viewRedownloads`

`int64`

Redownloads from people who viewed your ad, but didn’t tap it, within a 1-day attribution window. The API counts redownloads when someone downloads your app, deletes it, and downloads it again on the same device, or a different one, following an ad view.

## Mentioned in 

Apple Search Ads Campaign Management API 2

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

