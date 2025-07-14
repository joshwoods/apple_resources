

- App Store Receipts
- App Store receipt data types
-  is_trial_period Deprecated

Type

# is_trial_period

An indicator of whether an auto-renewable subscription is in the free trial period.

App Store Receipts 1.0–1.7Deprecated

``` source
string is_trial_period
```

## Possible Values 

`true`  

The subscription is in the free trial period.

`false`  

The subscription is not in the free trial period.

## Discussion

This field is returned in the JSON response, in the responseBody.Latest_receipt_info and responseBody.Receipt.In_app arrays.

You can use this value to determine whether the specific record is in a subscription trial period. If a previous subscription period in the receipt has the value `"true" `for either the `is_trial_period` or is_in_intro_offer_period keys, the user is not eligible for a free trial or introductory price within that subscription group.

## See Also

### Receipt and subscription status

type status

The status of the app receipt.

Deprecated

type auto_renew_status

The renewal status for the auto-renewable subscription.

Deprecated

type is_in_billing_retry_period

An indicator of whether an auto-renewable subscription is in the billing retry period.

Deprecated

type is_in_intro_offer_period

An indicator of whether an auto-renewable subscription is in the introductory price period.

Deprecated

