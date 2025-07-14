

- Apple Search Ads
-  ReportingKeyword 

Object

# ReportingKeyword

The response to a request to fetch keyword-level reports.

Search Ads 2.0+

``` source
object ReportingKeyword
```

## Properties

`adGroupDeleted`

`boolean`

An indicator of whether the ad group is soft-deleted.

You can use the `EQUALS` and `IN` selector Condition operators with Get Keyword-Level Reports.

`adGroupId`

`int64`

The unique identifier for the ad group.

You can use the `EQUALS`, `IN`, and `STARTSWITH` selector Condition operators with Get Keyword-Level Reports.

`adGroupName`

`string`

The name of the ad group, which is unique within the campaign. Responses don’t include deleted ad groups.

You can use the `EQUALS`, `IN`, and `STARTSWITH` selector Condition operators with Get Keyword-Level Reports.

`bidAmount`

Money

This is the offer price for a keyword in a bidding auction. If the `bidAmount` field is `null`, the `bidAmount` uses the `defaultBidAmount` of the corresponding ad group.

`campaignId`

`int64`

The unique identifier for the campaign.

You can use the `EQUALS`, `IN`, and `STARTSWITH` Selector Condition operators with Get Keyword-Level Reports.

`deleted`

`boolean`

An indicator of whether the keyword is soft-deleted.

You can use the `EQUALS` and `IN` selector Condition operators with Get Keyword-Level Reports.

`keyword`

`string`

The name of a keyword that belongs to an ad group.

You can use the `EQUALS`, `IN`, and `STARTSWITH` selector Condition operators with Get Keyword-Level Reports.

`keywordDisplayStatus`

`string`

The state of the keyword display operation.

You can use the `EQUALS` and `IN` selector Condition operators with Get Keyword-Level Reports.

Possible Values: `AD_GROUP_ON_HOLD, CAMPAIGN_ON_HOLD, DELETED, PAUSED, RUNNING`

`keywordId`

`int64`

The unique identifier of a keyword that belongs to an ad group.

`keywordStatus`

`string`

The status of the keyword.

Possible Values: `ACTIVE, PAUSED`

`matchType`

`string`

An automated keyword and bidding strategy. See Ad Groups for Search Match use cases.

`Auto`  
Specifies the system serves impressions with optimized keywords, in addition to those you explicitly add to the ad group.

`Broad`  
Ensures your ads don’t run on relevant, close variants of a keyword, such as singulars, plurals, misspellings, synonyms, related searches, and phrases that include that term (fully or partially).

`Exact`  
Offers the most control over searches your ad may appear in. You can target a specific term and its close variants, such as common misspellings and plurals. Your ad may receive fewer impressions as a result, but your tap-through rates (TTRs) and conversions on those impressions may be higher because you’re reaching users most interested in your app.

You can use the `EQUALS` selector Condition operator with Get Keyword-Level Reports.

Possible Values: `AUTO, BROAD, EXACT`

`modificationTime`

`date-time`

The date and time of the most recent modification of the object.

`orgId`

`int64`

The identifier of the organization that owns the campaign. Your `orgId` is the same as your account in the Apple Search Ads UI.

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

