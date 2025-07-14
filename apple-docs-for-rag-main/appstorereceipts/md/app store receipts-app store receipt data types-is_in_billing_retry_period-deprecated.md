

- App Store Receipts
- App Store receipt data types
-  is_in_billing_retry_period Deprecated

Type

# is_in_billing_retry_period

An indicator of whether an auto-renewable subscription is in the billing retry period.

App Store Receipts 1.0–1.7Deprecated

``` source
string is_in_billing_retry_period
```

## Possible Values 

`1`  

The App Store is attempting to renew the subscription.

`0`  

The App Store has stopped attempting to renew the subscription.

## Discussion

This field is returned in the JSON response, in the responseBody.Pending_renewal_info array.

This field indicates whether Apple is attempting to renew an expired subscription automatically. If the customer’s subscription failed to renew because the App Store was unable to complete the transaction, this value reflects whether the App Store is still trying to renew the subscription.

The subscription retry flag is solely indicative of whether a subscription is in a billing retry state. Use this value in conjunction with `expiration_intent`, `expires_date`, and `transaction_id` for more insight.

You can use this field to:

- Determine that the user has been billed successfully, if this field has been removed and there is a new transaction with a future `expires_date`.

- Inform the user that there may be an issue with their billing information, if the value is `“1”`. For example, an expired credit card or insufficient balance could prevent this customer's account from being billed.

- Implement a grace period to improve recovery, if the value is `“1”` and the `expires_date` is in the past. A grace period is free or limited subscription access while a subscriber is in a billing retry state. See Engineering Subscriptions from WWDC 2018 for more information.

## See Also

### Receipt and subscription status

type status

The status of the app receipt.

Deprecated

type auto_renew_status

The renewal status for the auto-renewable subscription.

Deprecated

type is_in_intro_offer_period

An indicator of whether an auto-renewable subscription is in the introductory price period.

Deprecated

type is_trial_period

An indicator of whether an auto-renewable subscription is in the free trial period.

Deprecated

