

- Apple Search Ads
- Campaign
-  Campaign.CountryOrRegionServingStateReasons 

Object

# Campaign.CountryOrRegionServingStateReasons

Reasons why a campaign can’t run.

Search Ads 2.0+

``` source
object Campaign.CountryOrRegionServingStateReasons
```

## Properties

`Any Key`

`[string]`

 (Read-only) 

A map of reasons that returns when a campaign can’t run for a specified country or region.

Possible Values: `ACCOUNT_DOC_APPROVAL_EXPIRED, ACCOUNT_DOC_APPROVAL_INFECTED, ACCOUNT_DOC_APPROVAL_NOT_SUBMITTED, ACCOUNT_DOC_APPROVAL_PENDING, ACCOUNT_DOC_APPROVAL_REJECTED, APP_CONTENT_REJECTED, APP_CONTENT_REVIEW_PENDING, APP_DOC_APPROVAL_EXPIRED, APP_DOC_APPROVAL_INFECTED, APP_DOC_APPROVAL_NOT_SUBMITTED, APP_DOC_APPROVAL_PENDING, APP_DOC_APPROVAL_REJECTED, APP_NOT_ELIGIBLE, APP_NOT_ELIGIBLE_SEARCHADS, APP_NOT_ELIGIBLE_SUPPLY_SOURCE, APP_NOT_PUBLISHED_YET, FEATURE_NOT_AVAILABLE_IN_COUNTRY_OR_REGION, SAPIN_LAW_AGENT_UNKNOWN, SAPIN_LAW_FRENCH_BIZ, SAPIN_LAW_FRENCH_BIZ_UNKNOWN`

## See Also

### Campaign Request and Response Objects

object Campaign

The response to a request to create and fetch campaigns.

object CampaignResponse

A container for the campaign response body.

object CampaignListResponse

The response details of campaign requests.

object CampaignUpdate

The list of campaign fields that are updatable.

object UpdateCampaignRequest

The payload properties to clear geotargeting from a campaign.

