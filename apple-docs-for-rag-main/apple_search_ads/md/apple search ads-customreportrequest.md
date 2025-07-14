

- Apple Search Ads
-  CustomReportRequest 

Object

# CustomReportRequest

The Impression Share report request body.

Search Ads 4.7+

``` source
object CustomReportRequest
```

## Properties

`dateRange`

`string`

The date range of the report request. A date range is required only when using `WEEKLY` granularity in Impression Share Report.

Default: `LAST_WEEK`

Possible Values: `LAST_WEEK, LAST_2_WEEKS, LAST_4_WEEKS`

`endTime`

`string`

The end time of the report. The format is `YYYY-MM-DD`, such as `2024-06-30`.

`granularity`

`string`

The report data organized by day or week.

Impression Share reports with a `WEEKLY` granularity value can’t have custom `startTime` and `endTime` in the request payload.

Default: `DAILY`

Possible Values: `DAILY, WEEKLY`

`name`

`string`

 (Required) 

A free-text field. The maximum length is 50 characters.

`selector`

CustomReportRequest.Selector

Selector is an optional parameter to filter API results using the CountryOrRegion and `adamId` fields. For CountryOrRegion, use an alpha-2 country code value. The `IN` operator is available to use with Impression Share reports.

See SovCondition for Selector descriptions and see Selector for structural guidance with selectors.

```
{
  "name": "impression_share_API_report_example",
  "granularity": "DAILY",
  "startTime": "2024-01-11",
  "endTime": "2024-02-08",
  "selector": {
    "conditions": [
      {
        "field": "adamId",
        "operator": "IN",
        "values": [
          1252497129,
          282614216
        ]
      },
      {
        "field": "countryOrRegion",
        "operator": "IN",
        "values": [
          "US",
          "CA"
        ]
      }
    ]
  }
}
```

`startTime`

`string`

The start time of the report. The format is `YYYY-MM-DD`, such as `2024-06-01`.

## Discussion

See also Impression Share Report, Get a Single Impression Share Report, Get All Impression Share Reports, and CustomReportResponse.

## Topics

### Objects

object CustomReportRequest.Selector

A list of condition objects.

## See Also

### Impression Share Report Request and Response Objects

object CustomReportResponse

A container for Impression Share report metrics.

object CustomReportResponseBody

A container for the Impression Share report response body.

object SovCondition

The list of condition objects that allow users to filter a list of records.

