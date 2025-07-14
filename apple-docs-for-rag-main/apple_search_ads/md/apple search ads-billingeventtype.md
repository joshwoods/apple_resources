

- Apple Search Ads
-  BillingEventType 

Type

# BillingEventType

The type of billing event for a campaign.

Search Ads 4.0+

``` source
string BillingEventType
```

## Possible Values 

`TAPS`  

The cost to the advertiser is per tap.

`IMPRESSIONS`  

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

When the `supplySources` value is `APPSTORE_SEARCH_RESULTS` or `APPSTORE_SEARCH_TAB`, the `billingEvent` must be `TAPS.`

IMPRESSIONS  
The cost to the advertiser is per impression served.

## Discussion

See also Campaign object.

## See Also

### Data Types

type AdChannelType

The channel type of an ad in a campaign.

type CampaignCountryOrRegionsServingStateReasons

Reasons that displays when a campaign can’t run.

type CampaignDisplayStatus

The status of the campaign.

type CampaignServingStateReasons

Reasons the system provides when a campaign can’t run.

type CampaignServingStatus

The status of the campaign.

type CampaignStatus

The status of the campaign.

type PaymentModel

The payment model that you set.

type SupplySource

The ad placements for a campaign.

