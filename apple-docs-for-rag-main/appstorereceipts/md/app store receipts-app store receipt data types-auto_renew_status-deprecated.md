

- App Store Receipts
- App Store receipt data types
-  auto_renew_status Deprecated

Type

# auto_renew_status

The renewal status for the auto-renewable subscription.

App Store Receipts 1.0–1.7Deprecated

``` source
string auto_renew_status
```

## Possible Values 

`1`  

The subscription will renew at the end of the current subscription period.

`0`  

The customer has turned off automatic renewal for the subscription.

## Discussion

This field is returned in the JSON response, in the responseBody.Pending_renewal_info array.

The value for this field should not be interpreted as the customer’s subscription status. You can use this value to display an alternative subscription product in your app, such as a lower-level subscription plan to which the user can downgrade from their current plan.

Consider presenting an attractive upgrade or downgrade offer in the same subscription group, if the `auto_renew_status` value is `“0”`. See Engineering Subscriptions from WWDC 2018 for more information.

## See Also

### Receipt and subscription status

type status

The status of the app receipt.

Deprecated

type is_in_billing_retry_period

An indicator of whether an auto-renewable subscription is in the billing retry period.

Deprecated

type is_in_intro_offer_period

An indicator of whether an auto-renewable subscription is in the introductory price period.

Deprecated

type is_trial_period

An indicator of whether an auto-renewable subscription is in the free trial period.

Deprecated

