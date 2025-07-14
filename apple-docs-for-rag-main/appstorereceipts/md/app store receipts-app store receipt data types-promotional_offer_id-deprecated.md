

- App Store Receipts
- App Store receipt data types
-  promotional_offer_id Deprecated

Type

# promotional_offer_id

The identifier of the promotional offer for an auto-renewable subscription that the user redeems.

App Store Receipts 1.0–1.7Deprecated

``` source
string promotional_offer_id
```

## Discussion

This field is returned in the JSON response, in the responseBody.Latest_receipt_info and responseBody.Receipt.In_app arrays.

You provide this value in the Promotional Offer Identifier field when you create the promotional offer in App Store Connect. For more information, see Set up promotional offers for auto-renewable subscriptions.

You can use the promotional offer ID value to:

- Confirm that the sale of the subscription was from a promotional offer.

- Confirm which promotional offer the user redeemed.

- Keep track of the promotional offers that a user has redeemed to limit discounts you offer, according to your business model.

For more information on promotional offers, see Implementing promotional offers in your app.

## See Also

### Promotions and offers

type offer_code_ref_name

The offer-reference name of the subscription offer code that the customer redeems.

Deprecated

