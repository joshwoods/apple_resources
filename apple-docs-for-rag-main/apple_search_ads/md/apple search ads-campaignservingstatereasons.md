

- Apple Search Ads
-  CampaignServingStateReasons 

Type

# CampaignServingStateReasons

Reasons the system provides when a campaign can’t run.

Search Ads 4.0+

``` source
string CampaignServingStateReasons
```

## Possible Values 

`AD_GROUP_MISSING`  

The ad group is missing from the campaign.

`APP_LANGUAGE_INCOMPATIBLE`  

The app language is not supported.

`APP_NOT_CATEGORIZED`  

The app doesn’t have an assigned category.

`APP_NOT_ELIGIBLE`  

The app isn’t eligible in App Store Connect.

`APP_NOT_ELIGIBLE_SEARCHADS`  

The app isn’t eligible for Apple Search Ads.

`APP_NOT_ELIGIBLE_SUPPLY_SOURCE`  

The app isn’t eligible for promotion with the supply source.

`APP_NOT_LINKED_TO_CAMPAIGN_GROUP`  

The app is no longer associated with any of the content providers linked to the campaign group.

`APP_NOT_PUBLISHED_YET`  

The app hasn’t been published on the App Store.

`APP_SENSITIVE_CONTENT`  

The app isn’t eligible due to the sensitive content policy.

`BO_START_DATE_IN_FUTURE`  

The budget order start date is in the future.

`BO_END_DATE_REACHED`  

The budget order end date is in the past.

`BO_EXHAUSTED`  

The budget order is exhausted.

`CAMPAIGN_END_DATE_REACHED`  

The campaign end date is in the past.

`CAMPAIGN_START_DATE_IN_FUTURE`  

The campaign start date is in the future.

`CONTENT_PROVIDER_UNLINKED`  

The app’s content provider isn’t linked to the campaign group.

`CREDIT_CARD_DECLINED`  

The system has declined the credit card charge.

`DAILY_CAP_EXHAUSTED`  

The campaign daily cap is exhausted.

`DELETED_BY_USER`  

The user has deleted the campaign.

`FEATURE_NO_LONGER_AVAILABLE`  

A pricing model of CPT isn’t available. See section 4.4 in Apple Search Ads Campaign Management API 4 for additional details.

`FEATURE_NOT_YET_AVAILABLE`  

A feature isn’t yet available.

`INELIGIBLE_BUSINESS_LOCATION`  

The account business profile location isn’t eligible.

`LOC_EXHAUSTED`  

The line of credit is exhausted.

`MISSING_BO_OR_INVOICING_FIELDS`  

The budget order is missing or has missing fields.

`NO_AVAILABLE_AD_GROUPS`  

The campaign has no ad groups running.

`NO_ELIGIBLE_COUNTRIES`  

The campaign has no eligible countries for the campaign to run.

`NO_PAYMENT_METHOD_ON_FILE`  

The organization doesn’t have a payment method. See BudgetOrder.

`ORG_CHARGE_BACK_DISPUTED`  

The organization has a disputed chargeback.

`ORG_PAYMENT_TYPE_CHANGED`  

The organization’s payment type has changed.

`ORG_SUSPENDED_POLICY_VIOLATION`  

The organization can’t run a campaign.

`ORG_SUSPENDED_FRAUD`  

The organization can’t run a campaign.

`PAUSED_BY_USER`  

The user has paused the campaign.

`PAUSED_BY_SYSTEM`  

The system has paused the campaign.

`SAPIN_LAW_AGENT_UNKNOWN`  

An agency hasn’t identified as an agency through their Search Ads account.

`SAPIN_LAW_FRENCH_BIZ_UNKNOWN`  

An app is owned by a business that is headquartered or has a branch in France, but hasn’t self-identified as an agency in their Search Ads account.

`SAPIN_LAW_FRENCH_BIZ`  

An app is owned by a business that is headquartered or has a branch in France, and has self-identified as an agency in their Search Ads account.

`TAX_VERIFICATION_PENDING`  

The organization’s tax verification is pending.

`TOTAL_BUDGET_EXHAUSTED`  

The campaign budget is exhausted.

`USER_REQUESTED_ACCOUNT_SUSPENSION`  

The user requested suspension of the account.

## Discussion

Ad creatives in campaigns with an `APPSTORE_TODAY_TAB` SupplySource receive a review from Apple for compliance. Ads that are pending review are on hold until Apple completes the review. The system doesn’t serve rejected ads.

## See Also

### Data Types

type AdChannelType

The channel type of an ad in a campaign.

type BillingEventType

The type of billing event for a campaign.

type CampaignCountryOrRegionsServingStateReasons

Reasons that displays when a campaign can’t run.

type CampaignDisplayStatus

The status of the campaign.

type CampaignServingStatus

The status of the campaign.

type CampaignStatus

The status of the campaign.

type PaymentModel

The payment model that you set.

type SupplySource

The ad placements for a campaign.

