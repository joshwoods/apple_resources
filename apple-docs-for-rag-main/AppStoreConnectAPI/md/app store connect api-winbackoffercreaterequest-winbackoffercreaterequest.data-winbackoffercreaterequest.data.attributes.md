

- App Store Connect API
- WinBackOfferCreateRequest
- WinBackOfferCreateRequest.Data
-  WinBackOfferCreateRequest.Data.Attributes 

Object

# WinBackOfferCreateRequest.Data.Attributes

Attributes that describe a winback offer resource.

App Store Connect API 3.6+

``` source
object WinBackOfferCreateRequest.Data.Attributes
```

## Properties

`customerEligibilityPaidSubscriptionDurationInMonths`

`integer`

 (Required) 

How long a customer was a subscriber. Possible values:

`1-24`  
1 to 24 months, as integers

`36`  
3 years

`48`  
4 years

`60`  
5 years

`customerEligibilityTimeSinceLastSubscribedInMonths`

IntegerRange

 (Required) 

How long since the subscribe last had an active subscription.

`customerEligibilityWaitBetweenOffersInMonths`

`integer`

How long since the subscribe last had an active subscription.

`duration`

SubscriptionOfferDuration

 (Required) 

The length of time for the offer period.

`endDate`

`date`

Minimum length for a win-back offer is 3 days.

`offerId`

`string`

 (Required) 

(Required) string of alphanumeric characters, periods, and underscores, up to 100 characters. Use a unique value that you have not used for a promotional offer, offer code, or introductory offer, when you create your win-back offer.

`offerMode`

SubscriptionOfferMode

 (Required) 

(Required) Describes how payment is configured for a win-back offer.

`periodCount`

`integer`

 (Required) 

(Required) The number of subscription duration intervals.

`priority`

`string`

 (Required) 

Select how this offer ranks among your other offers and in-app events. `HIGH` priority offers will appear above other offers and events on your appʼs product page.

Possible Values: `HIGH, NORMAL`

`promotionIntent`

`string`

You can promote this offer on your App Store product page. Promoted offers can also display in search results and may be featured on the Today, Games, and Apps tabs. If your win-back offer is live and `promotionIntent` is set to `USE_AUTO_GENERATED_ASSETS` you need to delete the win-back offer in order to remove it from promotion.

Possible Values: `NOT_PROMOTED, USE_AUTO_GENERATED_ASSETS`

`referenceName`

`string`

 (Required) 

A string of alphanumeric characters, spaces, periods, and underscores, up to 65 characters. Use a unique value that you have not used for a promotional offer, offer code, or introductory offer, when you create your win-back offer.

`startDate`

`date`

 (Required) 

First available date is today + 1 day.

## Mentioned in 

Creating and configuring win-back offers

## See Also

### Objects

object WinBackOfferCreateRequest.Data.Relationships

The relationships you included in the request and those on which you can operate.

