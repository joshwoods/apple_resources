

- Apple Search Ads
-  ReportingCampaign 

Object

# ReportingCampaign

The response to a request to fetch campaign-level reports.

Search Ads 2.0+

``` source
object ReportingCampaign
```

## Properties

`adChannelType`

`string`

The channel type of ad in a campaign.

See AdChannelType for value descriptions.

You can use the `EQUALS` Selector Condition operator with Get Campaign-Level Reports.

Possible Values: `SEARCH, DISPLAY`

`app`

CampaignAppDetail

The name of the app and the `adamId`.

`campaignId`

`int64`

The identifier for the campaign.

You can use the `EQUALS`, `IN`, and `STARTSWITH` Selector Condition operators with Get Campaign-Level Reports.

`campaignName`

`string`

The unique name of the campaign.

You can use the `EQUALS`, `IN`, and `STARTSWITH` Selector Condition operators with Get Campaign-Level Reports.

`campaignStatus`

`string`

The status of the campaign.

See CampaignStatus for value descriptions.

You can use the `EQUALS` Selector Condition operator with Get Campaign-Level Reports.

Possible Values: `ENABLED, PAUSED`

`countriesOrRegions`

`[string]`

The App Store geoterritories where you’re promoting your app.

This field requires an ISO 3166-1 alpha-2 country code value for the locations where you’re promoting. The default value is `US`.

You can use the `EQUALS`, `CONTAINS_ANY`, and `CONTAINS_ALL` Selector Condition operators with Get Campaign-Level Reports.

`countryOrRegionServingStateReasons`

ReportingCampaign.CountryOrRegionServingStateReasons

The map of reasons that returns when a campaign isn’t running.

`dailyBudget`

Money

The daily budget amount available to the campaign. This is the equivalent of `dailyBudgetAmount` in your Campaign.

`deleted`

`boolean`

The indicator of whether the campaign is soft-deleted.

You can use the `EQUALS` and `IN` Selector Condition operators with Get Campaign-Level Reports.

`displayStatus`

`string`

The status of the campaign. The status resolves according to `servingStatus` and additional criteria.

Possible Values: `DELETED, ON_HOLD, PAUSED, RUNNING`

`modificationTime`

`date-time`

The date and time of the most recent modification of the object.

`orgId`

`int64`

The identifier of the organization that owns the campaign. Your `orgId` is the same as your account in the Apple Search Ads UI.

`servingStateReasons`

`[string]`

A list of reasons that displays when a campaign can’t run.

See CampaignServingStateReasons for value descriptions.

Possible Values: `AD_GROUP_MISSING, APP_NOT_CATEGORIZED, APP_NOT_ELIGIBLE, APP_NOT_ELIGIBLE_SEARCHADS, APP_NOT_ELIGIBLE_SUPPLY_SOURCE, APP_NOT_LINKED_TO_CAMPAIGN_GROUP, APP_NOT_PUBLISHED_YET, APP_SENSITIVE_CONTENT, BO_END_DATE_REACHED, BO_EXHAUSTED, BO_START_DATE_IN_FUTURE, CAMPAIGN_END_DATE_REACHED, CAMPAIGN_START_DATE_IN_FUTURE, CONTENT_PROVIDER_UNLINKED, CREDIT_CARD_DECLINED, DAILY_CAP_EXHAUSTED, DELETED_BY_USER, FEATURE_NOT_YET_AVAILABLE, FEATURE_NO_LONGER_AVAILABLE, INELIGIBLE_BUSINESS_LOCATION, LOC_EXHAUSTED, MISSING_BO_OR_INVOICING_FIELDS, NO_AVAILABLE_AD_GROUPS, NO_ELIGIBLE_COUNTRIES, NO_PAYMENT_METHOD_ON_FILE, ORG_CHARGE_BACK_DISPUTED, ORG_PAYMENT_TYPE_CHANGED, ORG_SUSPENDED_FRAUD, ORG_SUSPENDED_POLICY_VIOLATION, PAUSED_BY_SYSTEM, PAUSED_BY_USER, SAPIN_LAW_AGENT_UNKNOWN, SAPIN_LAW_FRENCH_BIZ, SAPIN_LAW_FRENCH_BIZ_UNKNOWN, TAX_VERIFICATION_PENDING, TOTAL_BUDGET_EXHAUSTED, USER_REQUESTED_ACCOUNT_SUSPENSION`

`servingStatus`

`string`

The status of the campaign.

You can use the `EQUALS` Selector Condition operator with Get Campaign-Level Reports.

Possible Values: `NOT_RUNNING, RUNNING`

`supplySources`

`[string]`

The ad placements for a campaign.

See SupplySource for value descriptions and validations.

You can use the `CONTAINS_ANY`, `CONTAINS_ALL`, and `EQUALS` Selector Condition operators with Get Campaign-Level Reports.

Possible Values: `APPSTORE_PRODUCT_PAGES_BROWSE, APPSTORE_SEARCH_RESULTS, APPSTORE_SEARCH_TAB, APPSTORE_TODAY_TAB`

`totalBudget`

Money

The total campaign budget amount. This is the equivalent of `budgetAmount` in your Campaign.

## Mentioned in 

Apple Search Ads Campaign Management API 2

## Topics

### Objects

object Campaign.CountryOrRegionServingStateReasons

Reasons why a campaign can’t run.

### Dictionaries

object ReportingCampaign.CountryOrRegionServingStateReasons

Reasons that return when a campaign can’t run.

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

