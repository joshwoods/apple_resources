

- Apple Search Ads
-  AdGroup 

Object

# AdGroup

The response to ad group requests.

Search Ads 2.0+

``` source
object AdGroup
```

## Properties

`automatedKeywordsOptIn`

`boolean`

The parameter for enabling and disabling Search Match. If `true`, the system automatically adds optimized keywords in addition to those you explicitly add to the ad group.

See the Enable and Disable Search Match section of Ad Groups.

You can use the `EQUALS` selector Condition operator with Find Ad Groups.

`campaignId`

`int64`

The unique identifier for a campaign.

You can use the `EQUALS`, `IN`, and `STARTSWITH` selector Condition operators with Find Ad Groups.

`cpaGoal`

Money

The cost-per-acquisition goal.

Important

You can update the `cpaGoal` only in campaigns that use the `APPSTORE_SEARCH_RESULTS` supply source.

`creationTime`

`date-time`

 (Read-only) 

The timestamp for the creation of the report in the format of `YYYY-MM-DD’T’HH:mm:ss.SSS`.

`defaultBidAmount`

Money

 (Required) 

The default maximum cost-per-tap or cost-per-impression bid for the ad group.

You can use the `EQUALS, GREATER_THAN, and LESS_THAN` selector Condition operators with Find Ad Groups.

`deleted`

`boolean`

 (Read-only) 

The indicator of whether the ad group is soft-deleted. This includes keywords that belong to an ad group.

You can use the `EQUALS` and `IN` selector Condition operators with Find Ad Groups.

Default: `false`

`displayStatus`

`string`

 (Read-only) 

The status of the ad group. The status resolves according to `servingStatus` and additional criteria.

Possible Values: `DELETED, ON_HOLD, PAUSED, RUNNING`

`endTime`

`date-time`

The scheduled end time and date for the ad group, which the system determines from the ad group with the latest end time.

- The `endTime` must be after the `startTime`.

- The `endTime` is updatable until you reach the designated time.

- The `endTime` must be in UTC.

`id`

`int64`

 (Read-only) 

The unique identifier for the ad group that you can use as `adGroupId` in endpoint resources.

You can use the `EQUALS`, `IN`, and `STARTSWITH` selector Condition operators with Find Ad Groups.

Minimum: `0`

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the object.

`name`

`string`

 (Required) 

The unique name of the ad group. Responses don’t include deleted ad groups.

You can use the `EQUALS`, `IN`, and `STARTSWITH` selector Condition operators with Find Ad Groups.

`orgId`

`int64`

The identifier of the organization that owns the campaign. Your `orgId` is the same as your account in the Search Ads UI.

`paymentModel`

`string`

The payment model that you set through the Search Ads UI. If you don’t set a payment model, campaigns can’t run.

See PaymentModel for value descriptions.

If you don’t select a payment model, you can still create campaigns. You must select a payment model before a campaign is eligible to run.

See BudgetOrder for details about setting a payment model.

Possible Values: `LOC, PAYG`

`pricingModel`

`string`

 (Required) 

The type of pricing model for a bid. See PricingModel for value descriptions.

Possible Values: `CPC, CPM`

`servingStateReasons`

`[string]`

 (Read-only) 

A list of reasons that displays when an ad group isn’t running.

Possible Values: `ADGROUP_END_DATE_REACHED, AD_GROUP_PAUSED_BY_USER, APP_NOT_SUPPORT, AUDIENCE_BELOW_THRESHOLD, CAMPAIGN_END_DATE_REACHED, CAMPAIGN_NOT_RUNNING, CAMPAIGN_START_DATE_IN_FUTURE, DELETED_BY_USER, NO_AVAILABLE_ADS, PENDING_AUDIENCE_VERIFICATION, START_DATE_IN_THE_FUTURE, TARGETED_DEVICE_CLASS_NOT_SUPPORTED_SUPPLY_SOURCE`

`servingStatus`

`string`

 (Read-only) 

The status of whether the ad group is serving.

Default: `RUNNING`

Possible Values: `NOT_RUNNING, RUNNING`

`startTime`

`date-time`

 (Required) 

The scheduled start date and time for the ad group with the earliest start time in the campaign.

- The `startTime` must be greater than the current time, and before the campaign `endTime`, if you set it.

- If you don’t set a `startTime`, the campaign defaults to the campaign request timestamp and the `startTime` is updatable until you reach the designated time.

- The `startTime` must be in UTC.

`status`

`string`

The user-controlled status to enable or pause the ad group.

This field is updatable.

You can use the `EQUALS` selector Condition operator with Find Ad Groups.

Default: `ENABLED`

Possible Values: `ENABLED, PAUSED`

`targetingDimensions`

TargetingDimensions

The targeting criteria to narrow the audience.

## Mentioned in 

Apple Search Ads Campaign Management API 4

## See Also

### Ad Group Request and Response Objects

object AdGroupUpdate

The response to ad group update requests.

object AdGroupResponse

A container for the ad group response body.

object AdGroupListResponse

The response details of ad group requests.

