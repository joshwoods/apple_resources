

- Apple Search Ads
-  CustomReportResponse 

Object

# CustomReportResponse

A container for Impression Share report metrics.

Search Ads 4.7+

``` source
object CustomReportResponse
```

## Properties

`creationTime`

`string`

The timestamp for the creation of the report in the format of `YYYY-MM-DD’T’HH:mm:ss.SSS`.

`dimensions`

`[string]`

`adamId`  
Your unique App Store app identifier.

`appName`  
The name of the app.

CountryOrRegion  
The App Store geoterritory where you’re promoting your app.

`searchTerm`  
The search terms to use for app searches.

`downloadUri`

`string`

The report download link. The `state` of the report needs to be `COMPLETED` for a valid URL to return when calling Get a Single Impression Share Report or Get All Impression Share Reports. A response of `null` means the report generation is still in progress. URLs expire 90 seconds after creation. Reports remain active for 2 days.

`endTime`

`string`

The end time of the report. The format is `YYYY-MM-DD`, such as `2024-06-30`.

`granularity`

`string`

The report data organized by day or week.

Possible Values: `DAILY, WEEKLY`

`id`

`int64`

The report `id` is a unique identifier per report.

`metrics`

`[string]`

Impression Share is a daily aggregation with a range in deciles, such as 11–20% and 21–30%.

App impressions for search terms correlate by country or region and organization against the total requests for country- or region-search term combinations. Search terms need to have more than 10 impressions per day for inclusion in a daily Impression Share report.

`lowImpressionShare`  
If impression share is 11–20%,  `lowImpressionShare` is 0.11 and `highImpressionShare` is 0.2.

`highImpressionShare`  
If impression share is 91–100%,  `lowImpressionShare` is 0.91 and `highImpressionShare` is 1.

`rank`  
The ranking of your app in terms of impression share compared to other apps in the same countries or regions. The rank displays from `ONE` to `FIVE` or `GREATER_THAN_FIVE`, with `ONE` being the highest rank.

`searchPopularity`  
The total search volume of keyword popularity. The popularity of search terms is based on country or region. The ranking is 1–5, with 5 as the most search volume.

`modificationTime`

`string`

The most recent timestamp of report modifications in the format of `YYYY-MM-DD’T’HH:mm:ss.SSS`.

`name`

`string`

A free-text field. The maximum length is 50 characters.

`selector`

CustomReportResponse.Selector

Selector is an optional parameter to filter API results using the CountryOrRegion and `adamId` fields. For CountryOrRegion, use alpha-2 country code values. The `IN` operator is available to use with Impression Share reports.

See SovCondition for selector descriptions and see Selector for structural guidance with selectors.

`startTime`

`string`

The start time of the report. The format is `YYYY-MM-DD`, such as `2024-06-01`.

`state`

`string`

The state of the report.

A value of `COMPLETED` has a report link in the `downloadUri` field.

Possible Values: `QUEUED, PENDING, COMPLETED, FAILED`

## Discussion

See also Impression Share Report, Get a Single Impression Share Report, Get All Impression Share Reports, and CustomReportRequest.

## Topics

### Objects

object CustomReportResponse.Selector

A list of condition objects.

## See Also

### Impression Share Report Request and Response Objects

object CustomReportRequest

The Impression Share report request body.

object CustomReportResponseBody

A container for the Impression Share report response body.

object SovCondition

The list of condition objects that allow users to filter a list of records.

