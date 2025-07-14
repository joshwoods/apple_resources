

- Apple Search Ads
-  Row 

Object

# Row

The report metrics by time granularity.

Search Ads 2.0+

``` source
object Row
```

## Properties

`insights`

InsightsObject

The bid recommendations according to currency type, including range and amount. See KeywordInsights and Get Keyword-Level Reports.

`granularity`

`[`ExtendedSpendRow`]`

The report data organized by hour, day, week, and month.

Note: If you specify `granularity` in the payload, `returnRowTotals` and `returnGrandTotals` must be `false`. See the payload example with granularity in Get Campaign-Level Reports.

`HOURLY`  
The `startTime` and `endTime` are ≤ 7 days apart, and the `startTime` is ≤ 30 days in the past.

Use: “`granularity": "HOURLY",`

The hour, `00` to `23`, appends to the date string as `HH`.

Note: `HOURLY` isn’t available to use in keyword reports, search term reports, or Creative Set reports.

`DAILY`  
The `startTime` and `endTime` are ≤ 90 days apart, and the `startTime` is ≤ 90 days in the past.

Use: `"granularity": "DAILY"`,

`WEEKLY`  
The `date` value is the Monday of the designated week.

The `startTime` and `endTime` are \> 14 days and ≤ 365 days apart, and the `startTime` is ≤ 24 months in the past.

Use: `"granularity": "WEEKLY",`

`MONTHLY`  
The `date` value is the first day of the designated month.

The `startTime` and `endTime` are \> 3 months apart, and the `startTime` is ≤ 24 months in the past.

Use: `"granularity": "MONTHLY",`

`metadata`

MetaDataObject

Reporting request data.

`other`

`boolean`

The impressions that return in reports when there are fewer than 100 demographic dimensions, and fewer than 10 search terms. If `other` is `true`, the corresponding dimensions are `null`.

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

object GrandTotalsRow

The summary of cumulative metrics.

object SpendRow

The reporting response metrics.

object ExtendedSpendRow

The descriptions of metrics with dates.

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

