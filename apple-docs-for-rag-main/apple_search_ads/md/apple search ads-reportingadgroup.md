

- Apple Search Ads
-  ReportingAdGroup 

Object

# ReportingAdGroup

The response to a request to fetch ad group-level reports.

Search Ads 2.0+

``` source
object ReportingAdGroup
```

## Properties

`adGroupDisplayStatus`

`string`

The state of the operation.

See AdGroupDisplayStatus for enum descriptions.

Possible Values: `CAMPAIGN_ON_HOLD, DELETED, ON_HOLD, PAUSED, RUNNING`

`adGroupId`

`int64`

The identifier for the ad group.

You can use the `EQUALS`, `IN`, and `STARTSWITH` Selector Condition operators with Get Ad Group-Level Reports.

`adGroupName`

`string`

The name of the ad group. This is unique within the campaign. Reports don’t include deleted ad groups.

You can use the `EQUALS`, `IN`, and `STARTSWITH` Selector Condition operators with Get Ad Group-Level Reports.

`adGroupServingStateReasons`

`[string]`

A list of reasons that displays when an ad group isn’t running.

See AdGroupServingStateReasons for enum descriptions.

Possible Values: `ADGROUP_END_DATE_REACHED, AD_GROUP_PAUSED_BY_USER, APP_NOT_SUPPORT, AUDIENCE_BELOW_THRESHOLD, CAMPAIGN_END_DATE_REACHED, CAMPAIGN_NOT_RUNNING, CAMPAIGN_START_DATE_IN_FUTURE, DELETED_BY_USER, NO_AVAILABLE_ADS, PENDING_AUDIENCE_VERIFICATION, START_DATE_IN_THE_FUTURE`

`adGroupServingStatus`

`string`

The status of whether the ad group is serving.

See AdGroupServingStatus for value descriptions.

Possible Values: `NOT_RUNNING, RUNNING`

`adGroupStatus`

`string`

The status of the ad group.

See AdGroupStatus for value descriptions.

You can use the `EQUALS` Selector Condition operator with Get Ad Group-Level Reports.

Possible Values: `ENABLED, PAUSED`

`automatedKeywordsOptIn`

`boolean`

The parameter for enabling and disabling Search Match. If `true`, the system automatically adds optimized keywords in addition to those you explicitly add to the ad group.

See the Enable and Disable Search Match section of Ad Groups.

You can use the `EQUALS` Selector Condition operator with Get Ad Group-Level Reports.

`campaignId`

`int64`

The unique identifier for the campaign.

You can use the `EQUALS`, `IN`, and `STARTSWITH` Selector Condition operators with Get Ad Group-Level Reports.

`cpaGoal`

Money

The cost-per-acquisition goal.

`defaultBidAmount`

Money

The default maximum cost per tap or impression bid for the ad group.

`deleted`

`boolean`

The indicator of whether the ad group is soft-deleted. This includes keywords that belong to an ad group.

You can use the `EQUALS` and `IN` Selector Condition operators with the Get Ad Group-Level Reports.

`endTime`

`date-time`

The scheduled end date and time for the ad group.

`modificationTime`

`date-time`

The date and time of the most recent modification of the object.

`orgId`

`int64`

The identifier of the organization that owns the campaign. Your `orgId` is the same as your account in the Apple Search Ads UI.

`startTime`

`date-time`

The scheduled start date and time for the ad group.

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

