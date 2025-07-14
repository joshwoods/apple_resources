

- Apple Search Ads
-  CampaignListResponse 

Object

# CampaignListResponse

The response details of campaign requests.

Search Ads 2.0+

``` source
object CampaignListResponse
```

## Properties

`data`

`[`Campaign`]`

Response data that the API provides.

`error`

ErrorResponseBody

Error response data that the API provides.

`pagination`

PageDetail

Page detail information that the API provides.

## See Also

### Campaign Request and Response Objects

object Campaign

The response to a request to create and fetch campaigns.

object CampaignResponse

A container for the campaign response body.

object Campaign.CountryOrRegionServingStateReasons

Reasons why a campaign can’t run.

object CampaignUpdate

The list of campaign fields that are updatable.

object UpdateCampaignRequest

The payload properties to clear geotargeting from a campaign.

