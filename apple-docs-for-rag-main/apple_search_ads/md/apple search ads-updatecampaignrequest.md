

- Apple Search Ads
-  UpdateCampaignRequest 

Object

# UpdateCampaignRequest

The payload properties to clear geotargeting from a campaign.

Search Ads 2.0+

``` source
object UpdateCampaignRequest
```

## Properties

`campaign`

CampaignUpdate

The campaign properties to update.

`clearGeoTargetingOnCountryOrRegionChange`

`boolean`

The parameter to clear geotargeting from all ad groups in the campaign. To modify `countriesOrRegions` in a campaign, set the value of `clearGeoTargetingOnCountryOrRegionChange` to `true`.

See the Payload Example: Update a Campaign with Countries or Regions in Update a Campaign.

Default: `false`

## See Also

### Campaign Request and Response Objects

object Campaign

The response to a request to create and fetch campaigns.

object CampaignResponse

A container for the campaign response body.

object Campaign.CountryOrRegionServingStateReasons

Reasons why a campaign can’t run.

object CampaignListResponse

The response details of campaign requests.

object CampaignUpdate

The list of campaign fields that are updatable.

