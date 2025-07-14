

- StoreKit
- Product
- Product.PurchaseOption
-  introductoryOfferEligibility(compactJWS:) 

Type Method

# introductoryOfferEligibility(compactJWS:)

Set the eligibility of an introductory offer for a purchase.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@backDeployed(before: iOS 18.4, macOS 15.4, tvOS 18.4, watchOS 11.4, visionOS 2.4)
static func introductoryOfferEligibility(compactJWS: String) -> Product.PurchaseOption
```

## Parameters 

`compactJWS`  

The signed JWT string with the introductory offer eligibility for the purchase.

