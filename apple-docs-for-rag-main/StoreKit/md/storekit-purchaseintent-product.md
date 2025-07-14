

- StoreKit
- PurchaseIntent
-  product 

Instance Property

# product

The product information of the In-App Purchase the customer selects to purchase outside of the app.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 14.4+

``` source
let product: Product
```

## Mentioned in 

Supporting win-back offers in your app

Supporting promoted In-App Purchases in your app

## Discussion

To enable users to complete the purchase they start on the App Store, call purchase(options:) on this product instance.

## See Also

### Identifying the product

var id: Product.ID

The product identifier of the In-App Purchase that the customer selects to purchase outside of the app.

