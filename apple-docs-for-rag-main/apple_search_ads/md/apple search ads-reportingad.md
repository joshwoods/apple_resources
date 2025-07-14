

- Apple Search Ads
-  ReportingAd 

Object

# ReportingAd

The response to a request to fetch ad-level reports.

Search Ads 4.0+

``` source
object ReportingAd
```

## Properties

`adDisplayStatus`

`string`

The `DisplayStatus` that derives from the ad’s serving status.

You can use the `EQUALS` and `IN` Selector Condition operators with Get Ad-Level Reports within a campaign.

Possible Values: `ACTIVE, INVALID, ON_HOLD, PAUSED, REMOVED`

`adGroupId`

`int64`

The unique identifier for the ad group the Creative belongs to.

You can use the `EQUALS` and `IN` Selector Condition operators with Get Ad-Level Reports within a campaign.

You can use this field with the `orderBy` selector.

`adId`

`int64`

A unique identifier that represents the assignment relationship between an ad group and an Ad.

You can use the `EQUALS`, `IN`, and `STARTSWITH` Selector Condition operators with Get Ad-Level Reports within a campaign.

`adName`

`string`

The unique name of a custom product page. The `adName` has to be unique within its ad group.

You can use this field with the `orderBy` selector.

`adServingStateReasons`

`string`

A list of reasons that displays when an ad isn’t running.

You can use this field with the `orderBy` selector.

Possible Values: `AD_APPROVAL_PENDING, AD_APPROVAL_REJECTED, DELETED_BY_USER, PAUSED_BY_SYSTEM, PAUSED_BY_USER, PRODUCT_PAGE_DELETED, PRODUCT_PAGE_HIDDEN, PRODUCT_PAGE_INCOMPATIBLE, PRODUCT_PAGE_INSUFFICIENT_ASSETS, AD_PROCESSING_IN_PROGRESS`

`campaignId`

`int64`

The unique identifier for a campaign.

You can use this field with the `orderBy` selector.

`creationTime`

`date-time`

The date and time of the creation of the Ad object.

You can use this field with the `orderBy` selector.

`creativeId`

`int64`

The unique identifier for a creative.

You can use the `EQUALS` and `IN` Selector Condition operators with Get Ad-Level Reports within a campaign.

`creativeType`

`string`

The type of creative asset. Synonymous with `type` in the Creative object.

You can use the `EQUALS` and `IN` Selector Condition operators with Get Ad-Level Reports within a campaign.

Possible Values: `CUSTOM_PRODUCT_PAGE, DEFAULT_PRODUCT_PAGE`

`deleted`

`boolean`

An indicator of whether a creative asset is soft-deleted..

You can use the `EQUALS` Selector Condition operators with Get Ad-Level Reports within a campaign.

`language`

`string`

The language of the Creative.

`modificationTime`

`date-time`

The date and time of the most recent modification of the object.

You can use this field with the `orderBy` selector.

`orgId`

`int64`

The identifier of the organization that owns the campaign. Your `orgId` is the same as your account in the Apple Search Ads UI.

You can use this field with the `orderBy` selector.

`productPageId`

`string`

A unique string to identify a product page on App Store Connect, such as `45812c9b-c296-43d3-c6a0-c5a02f74bf6e`.

`status`

`string`

The status of creative assets.

You can use this field with the `orderBy` selector.

Possible Values: `INVALID, VALID`

## Mentioned in 

Apple Search Ads Campaign Management API 4

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

object CampaignAppDetail

The app data to fetch from campaign-level reports.

object InsightsObject

The container object for bid recommendations.

object KeywordInsights

The object that contains bid recommendations.

