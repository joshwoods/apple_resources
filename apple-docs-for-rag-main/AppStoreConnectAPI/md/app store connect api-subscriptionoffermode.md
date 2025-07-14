

- App Store Connect API
-  SubscriptionOfferMode 

Type

# SubscriptionOfferMode

A string that indicates the payment mode of a subscription offer.

App Store Connect API 2.0+

``` source
string SubscriptionOfferMode
```

## Possible Values 

`PAY_AS_YOU_GO`  

`PAY_UP_FRONT`  

`FREE_TRIAL`  

## Discussion

### Possible alues

PAY_AS_YOU_GO  
A constant that indicates a subscription offer is billed over multiple billing periods.

PAY_UP_FRONT  
A constant that indicates a subscription offer is billed one time, up front.

FREE_TRIAL  
A constant that indicates a subscription offer is a free trial.

## See Also

### Objects and Types

object SubscriptionOfferCode.Attributes

type SubscriptionOfferDuration

A length of time that can be assigned to a subscription.

type SubscriptionOfferEligibility

type SubscriptionCustomerEligibility

object SubscriptionOfferCode.Relationships

