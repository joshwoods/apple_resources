

- App Store Receipts
- App Store receipt data types
-  in_app_ownership_type Deprecated

Type

# in_app_ownership_type

The relationship of the user with the family-shared purchase to which they have access.

App Store Receipts 1.4–1.7Deprecated

``` source
string in_app_ownership_type
```

## Possible Values 

`FAMILY_SHARED`  

The transaction belongs to a family member who benefits from service.

`PURCHASED`  

The transaction belongs to the purchaser.

## Discussion

When family members benefit from a shared subscription, App Store updates their receipt to include the family-shared purchase. Use the value of `in_app_ownership_type` to understand whether a transaction belongs to the purchaser or a family member who benefits.

This field appears in the App Store server notifications unified receipt (unified_receipt.Latest_receipt_info) and in transaction receipts (responseBody.Latest_receipt_info).

For more information about Family Sharing, see Supporting Family Sharing in your app.

