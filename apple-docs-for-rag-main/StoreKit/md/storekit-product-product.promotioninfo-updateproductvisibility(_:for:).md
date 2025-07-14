

- StoreKit
- Product
- Product.PromotionInfo
-  updateProductVisibility(\_:for:) 

Type Method

# updateProductVisibility(\_:for:)

Updates a value that indicates whether a promoted in-app purchase appears in the App Store on the user’s device.

iOS 16.4+iPadOS 16.4+

``` source
static func updateProductVisibility(
    _ visibility: Product.PromotionInfo.Visibility,
    for productID: Product.ID
) async throws
```

## Parameters 

`visibility`  

A visibility value of Product.PromotionInfo.Visibility that determines whether a promoted in-app purchase appears in the App Store on the user’s device.

`productID`  

The product identifier of the promoted in-app purchase.

## Mentioned in 

Supporting promoted In-App Purchases in your app

## Discussion

Call this method to change the visibility setting for a promoted in-app purchase. Changes take effect after you call this method.

The following code example updates a promoted product’s visibility after the user purchases it. The purchased product is hidden to avoid showing it again on the device.

```
// Update visibility to hide a promoted product after the user purchases it.
let purchasedProductIdentifier = "com.example.ExampleApp.product1"

do {
  try await Product.PromotionInfo.updateProductVisibility(.hidden, for: purchasedProductIdentifier)
}
catch {

}
```

## See Also

### Managing promotion visibility

var visibility: Product.PromotionInfo.Visibility

A value that indicates whether the promoted in-app purchase is visible or hidden on the user’s device.

enum Visibility

The visibility states for product promotion information.

