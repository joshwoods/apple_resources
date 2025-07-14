

- App Store Receipts
- App Store receipt data types
-  is_in_intro_offer_period Deprecated

Type

# is_in_intro_offer_period

An indicator of whether an auto-renewable subscription is in the introductory price period.

App Store Receipts 1.0–1.7Deprecated

``` source
string is_in_intro_offer_period
```

## Possible Values 

`true`  

The customer’s subscription is in an introductory price period

`false`  

The subscription is not in an introductory price period.

## Discussion

This field is returned in the JSON response, in the responseBody.Latest_receipt_info and responseBody.Receipt.In_app arrays.

You can use this value to determine if the user is eligible for introductory pricing. If a previous subscription period in the receipt has the value `“true”` for either the is_trial_period or `is_in_intro_offer_period` keys, the user is not eligible for a free trial or introductory price within that subscription group. For more information, see Implementing introductory offers in your app.

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

type is_trial_period

An indicator of whether an auto-renewable subscription is in the free trial period.

Deprecated

