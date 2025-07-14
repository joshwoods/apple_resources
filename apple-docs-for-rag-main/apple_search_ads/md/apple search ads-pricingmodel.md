

- Apple Search Ads
-  PricingModel 

Type

# PricingModel

The type of pricing model for a bid.

Search Ads 4.0+

``` source
string PricingModel
```

## Possible Values 

`CPC`  

The average cost for each ad tap in a campaign.

`CPM`  

The cost per 1000 impressions in a campaign.

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

Important

\> Apple Search Ads Campaign Management API 4.4 deprecates CPM. You can’t update CPM campaigns to CPC campaigns. You need to use CPC when creating a new campaign. See section 4.4 in Apple Search Ads Campaign Management API 4 for additional details.

## Discussion

See also AdChannelType, BillingEventType, and Campaign object. See Create a Campaign and Create an Ad Group for payload examples.

## See Also

### Data Types

type AdGroupDisplayStatus

The status of the ad group.

type AdGroupServingStateReasons

A list of reasons that displays when an ad group isn’t running.

type AdGroupServingStatus

The status of whether the ad group is serving.

type AdGroupStatus

The status of whether the ad group is enabled or not.

type DeviceClass

The defined targeted audience to include by device type.

type Gender

The defined targeted audience in a campaign.

