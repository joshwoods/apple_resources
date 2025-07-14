

- Apple Search Ads
-  ReportingRequest 

Object

# ReportingRequest

The report request body.

Search Ads 2.0+

``` source
object ReportingRequest
```

## Properties

`endTime`

`string`

 (Required) 

The date and time the report coverage ends. The format is `YYYY-MM-DD`.

`granularity`

`string`

The report data organized by hour, day, week, and month.

Note

For Get Search Term-Level Reports, if you specify `granularity` in the payload, make sure `returnRowTotals` and `returnGrandTotals` are `false`.

`HOURLY`  
The `startTime` and `endTime` are ≤ 7 days apart, and the `startTime` is ≤ 30 days in the past.

Use: `"granularity":"HOURLY"`,

The hour, `00` to `23`, appends to the date string as `HH`.

Note

`HOURLY` isn’t available to use in Get Search Term-Level Reports.

`DAILY`  
The `startTime` and `endTime` are ≤ 90 days apart, and the `startTime` is ≤ 90 days in the past.

`WEEKLY`  
The `date` value is the Monday of the designated week.

The `startTime` and `endTime` are \> 14 days and ≤ 365 days apart, and the `startTime` is ≤ 24 months in the past.

`MONTHLY`  
The `date` value is the first day of the designated month.

The `startTime` and `endTime` are \> 3 months apart, and the `startTime` is ≤ 24 months in the past.

Possible Values: `DAILY, HOURLY, MONTHLY, WEEKLY`

`groupBy`

`[string]`

Use the `groupBy` field to group responses by selected dimensions. If `groupBy` specifies age, gender, and geodimensions, `returnRowTotals` and `returnGrandTotals` must be `false`.

Note

The API groups `ageRange`, `countryCode`, Gender, `adminArea`, and `locality` records with fewer than 100 impressions in the API response as `other`.

The following `groupBy` descriptions include supported values per dimension:

`adminArea`  
The `adminArea` dimension is a group of states or the equivalent according to its associated `country`. Use Search for Geolocations to retrieve geolocations.

In Get Ad Group-Level Reports, you need to use the `adminArea` dimension with `countryCode`. The `locality` dimension is optional.

`ageRange`  
The `ageRange` dimension is a group of the user demographic age ranges.

In Get Ad Group-Level Reports, the `ageRange` dimension is available to use with DeviceClass.

`countryCode`  
The `countryCode` dimension is a group of country codes that indicate the country or region to serve ads in.

In Get Ad Group-Level Reports, the `countryCode` dimension is available to use with DeviceClass, `adminArea`, and `locality`.

CountryOrRegion  
The CountryOrRegion dimension is a group of countries and regions.

In Get Campaign-Level Reports, Get Ad Group-Level Reports, Get Keyword-Level Reports, and Get Search Term-Level Reports, the CountryOrRegion dimension is available to use with DeviceClass.

DeviceClass  
The DeviceClass dimension is a group of device classes that the promoted app supports.

In Get Ad Group-Level Reports, the DeviceClass dimension is available to use with any other dimension.

Gender  
The Gender dimension is a group of user-demographic genders.

In Get Ad Group-Level Reports, the Gender dimension is available to use with DeviceClass.

`locality`  
The `locality` dimension is the city or group of cities equivalent according to its associated `adminArea`. See Search for Geolocations to retrieve geolocations.

In Get Ad Group-Level Reports, the `locality` dimension with higher dimensions is available to use with `countryCode` and `adminArea`.

Possible Values: `adminArea, ageRange, countryCode, countryOrRegion, deviceClass, gender, locality`

`returnGrandTotals`

`boolean`

Returns the total of all the rows in the result set. If you don’t specify `granularity`, `returnRowTotals` must be `true`. If you specify `granularity` in the payload, `returnGrandTotals` must be `false`. The default is `false`.

`returnRecordsWithNoMetrics`

`boolean`

Specifies whether the API returns records without metrics. The default is `false`.

`returnRowTotals`

`boolean`

Specifies whether to return the totals of each row. If you don’t specify `granularity`, `returnRowTotals` must be `true`. If you specify `granularity` in the payload, `returnGrandTotals` must be `false`. The default is `false`. For example:

```
"granularity": "DAILY",
"returnRowTotals": false,
"returnGrandTotals": false
```

`selector`

Selector

 (Required) 

Selector objects define what data the API returns when fetching resources. Selector objects are available to use with Find and Reports endpoints.

Condition  
Additional types of filters to perform deeper filtering of the data.

For available conditions per field for each report type, see ReportingCampaign, ReportingAdGroup, ReportingKeyword, ReportingSearchTerm, and ReportingAd.

`orderBy`  
Specify a field name and grouping to sort the records by `ASCENDING` or `DESCENDING`.

This sorts on all `groupBy` dimensions and most metadata. See ExtendedSpendRow.

Only one `orderBy` field is available to use per payload.

Pagination  
Specify how many records to return per page. The default is `20`.

`startTime`

`string`

 (Required) 

The date and time the report coverage starts. The format is `YYYY-MM-DD`.

`timeZone`

`string`

You set the default `timeZone` during account creation through the Apple Search Ads UI. `ORTZ` (organization time zone) is the default.

Possible Values: `ORTZ, UTC`

## Mentioned in 

Apple Search Ads Campaign Management API 2

## See Also

### Reports Request and Response Objects

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

object KeywordInsights

The object that contains bid recommendations.

