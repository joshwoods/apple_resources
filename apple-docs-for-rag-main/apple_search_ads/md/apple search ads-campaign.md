

- Apple Search Ads
-  Campaign 

Object

# Campaign

The response to a request to create and fetch campaigns.

Search Ads 2.0+

``` source
object Campaign
```

## Properties

`adamId`

`int64`

 (Required) 

Your unique App Store app identifier. You can obtain your app `adamId` through Search for iOS apps, Get a Campaign, or Get all Campaigns.

You can use the `EQUALS` and `IN` selector Condition operators with Find Campaigns.

`adChannelType`

`string`

 (Required) 

The channel type of an ad in a campaign.

See AdChannelType for value descriptions.

You can use the `EQUALS` selector Condition operator with Find Campaigns and Get Campaign-Level Reports.

Possible Values: `SEARCH, DISPLAY`

`billingEvent`

`string`

 (Required) 

The type of billing event for a campaign.

See BillingEventType for value descriptions.

Possible Values: `IMPRESSIONS, TAPS`

`budgetAmount`

Money

The lifetime budget amount available to a campaign.

If you update a `budgetAmount`, the updated amount must be greater than the previous `budgetAmount` and must exceed the lifetime spend of the campaign.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` selector Condition operators with Find Campaigns.

This field is updatable.

`budgetOrders`

`[int64]`

The budget orders that you assign to the campaign. This applies only to campaigns with a line-of-credit payment model.

This field is updatable.

`countriesOrRegions`

`[string]`

 (Required) 

The App Store geoterritories where you’re promoting your app. The default value is `US`.

Use an alpha-2 country code value , such as `US`, for the locations where you’re promoting.

The `EQUALS`, `CONTAINS_ANY`, and `CONTAINS_ALL` selector Condition operators are available to use with Find Campaigns.

This field is updatable.

`countryOrRegionServingStateReasons`

Campaign.CountryOrRegionServingStateReasons

 (Read-only) 

The map of reasons that returns when a campaign isn’t running.

See CampaignCountryOrRegionsServingStateReasons for value descriptions.

`creationTime`

`date-time`

 (Read-only) 

The date and time of the creation of the `campaign` object.

`dailyBudgetAmount`

Money

 (Required) 

Your daily budget.

A `dailyBudgetAmount` is required field for all new campaigns, even if a `budgetAmount` is specified.

- A `dailyBudgetAmount` can be changed but not removed from the payload when updating an existing campaign.

- Your `dailyBudgetAmount` must be less than your `budgetAmount`.

- Your `dailyBudgetAmount` must be greater than or equal to the `defaultBidAmount` in your AdGroup.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` selector Condition operators with Find Campaigns.

This field is updatable.

`deleted`

`boolean`

 (Read-only) 

The indicator of whether the campaign is soft-deleted.

You can use the `EQUALS` and `IN` selector Condition operators with Find Campaigns.

Default: `false`

`displayStatus`

`string`

The status of the campaign. The status resolves according to `servingStatus` and additional criteria.

Possible Values: `DELETED, ON_HOLD, PAUSED, RUNNING`

`endTime`

`date-time`

 (Read-only) 

The scheduled end time and date for the campaign.

- The `endTime` must be after the `startTime`.

- The `endTime` is updatable until you reach the designated time.

- The `endTime` must be in UTC.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` selector Condition operators with Find Campaigns.

`id`

`int64`

 (Read-only) 

A unique identifier for the campaign that you can use as a `campaignid` in endpoint resources.

You can use the `EQUALS` and `IN` selector Condition operators with Find Campaigns.

`locInvoiceDetails`

LOCInvoiceDetails

The standard invoice details that you can set and edit using the LOCInvoiceDetails object.

This field is updatable.

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the object.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` selector Condition operators with Find Campaigns.

`name`

`string`

 (Required) 

The name of the campaign, which is unique within an organization.

You can use the `EQUALS`, `IN`, and `STARTSWITH` selector Condition operators with Find Campaigns.

This field is updatable.

Maximum length: `200`

`orgId`

`int64`

The identifier of the organization that owns the campaign. Your `orgId` is the same as your account in the Search Ads UI.

`paymentModel`

`string`

The payment model that you set through the Search Ads UI. If you don’t set a payment model, campaigns can’t run.

See PaymentModel for value descriptions.

If you don’t select a payment model, you can still create campaigns. You must select a payment model before a campaign is eligible to run.

See BudgetOrder for details about setting a payment model.

You can use the `EQUALS` and `IN` selector Condition operators with Find Campaigns.

Possible Values: `LOC, PAYG`

`servingStateReasons`

`[string]`

 (Read-only) 

A list of reasons that displays when a campaign can’t run.

See CampaignServingStateReasons for value descriptions.

Possible Values: `AD_GROUP_MISSING, APP_NOT_CATEGORIZED, APP_NOT_ELIGIBLE, APP_NOT_ELIGIBLE_SEARCHADS, APP_NOT_ELIGIBLE_SUPPLY_SOURCE, APP_NOT_LINKED_TO_CAMPAIGN_GROUP, APP_NOT_PUBLISHED_YET, APP_SENSITIVE_CONTENT, BO_END_DATE_REACHED, BO_EXHAUSTED, BO_START_DATE_IN_FUTURE, CAMPAIGN_END_DATE_REACHED, CAMPAIGN_START_DATE_IN_FUTURE, CONTENT_PROVIDER_UNLINKED, CREDIT_CARD_DECLINED, DAILY_CAP_EXHAUSTED, DELETED_BY_USER, FEATURE_NOT_YET_AVAILABLE, FEATURE_NO_LONGER_AVAILABLE, INELIGIBLE_BUSINESS_LOCATION, LOC_EXHAUSTED, MISSING_BO_OR_INVOICING_FIELDS, NO_AVAILABLE_AD_GROUPS, NO_ELIGIBLE_COUNTRIES, NO_PAYMENT_METHOD_ON_FILE, ORG_CHARGE_BACK_DISPUTED, ORG_PAYMENT_TYPE_CHANGED, ORG_SUSPENDED_FRAUD, ORG_SUSPENDED_POLICY_VIOLATION, PAUSED_BY_SYSTEM, PAUSED_BY_USER, SAPIN_LAW_AGENT_UNKNOWN, SAPIN_LAW_FRENCH_BIZ, SAPIN_LAW_FRENCH_BIZ_UNKNOWN, TAX_VERIFICATION_PENDING, TOTAL_BUDGET_EXHAUSTED, USER_REQUESTED_ACCOUNT_SUSPENSION`

`servingStatus`

`string`

 (Read-only) 

The status of the campaign.

You can use the `EQUALS` and `IN` selector Condition operators with Find Campaigns.

Possible Values: `RUNNING, NOT_RUNNING`

`startTime`

`date-time`

 (Read-only) 

The scheduled start time and date for the campaign.

- The `startTime` must be greater than the current time, and before the campaign `endTime`, if you set it.

- If you don’t set a `startTime`, the campaign defaults to the campaign request timestamp and the `startTime` is updatable until you reach the designated time.

- The `startTime` must be in UTC.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` selector Condition operators with Find Campaigns.

This field is updatable.

`status`

`string`

The user-controlled status to enable or pause the campaign.

You can use the `EQUALS` and `IN` selector Condition operators with Find Campaigns.

This field is updatable.

Default: `ENABLED`

Possible Values: `ENABLED, PAUSED`

`supplySources`

`[string]`

 (Required) 

The ad placements for a campaign.

See SupplySource for full descriptions of values.

You can use the `EQUALS` , `CONTAINS_ANY`, `CONTAINS_ALL` selector Condition operators with Find Campaigns.

Possible Values: `APPSTORE_PRODUCT_PAGES_BROWSE, APPSTORE_SEARCH_RESULTS, APPSTORE_SEARCH_TAB, APPSTORE_TODAY_TAB`

## Mentioned in 

Apple Search Ads Campaign Management API 4

Apple Search Ads Campaign Management API 2

## Topics

### Objects

object Campaign.CountryOrRegionServingStateReasons

Reasons why a campaign can’t run.

## See Also

### Campaign Request and Response Objects

object CampaignResponse

A container for the campaign response body.

object Campaign.CountryOrRegionServingStateReasons

Reasons why a campaign can’t run.

object CampaignListResponse

The response details of campaign requests.

object CampaignUpdate

The list of campaign fields that are updatable.

object UpdateCampaignRequest

The payload properties to clear geotargeting from a campaign.

