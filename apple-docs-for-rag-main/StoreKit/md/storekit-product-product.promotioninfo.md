

- StoreKit
- Product
-  Product.PromotionInfo 

Structure

# Product.PromotionInfo

Information about a promoted In-App Purchase that customizes its order and visibility on the device.

iOS 16.4+iPadOS 16.4+

``` source
struct PromotionInfo
```

## Mentioned in 

Supporting promoted In-App Purchases in your app

## Overview

The `Product.PromotionInfo` structure represents promoted in-app purchases available in your app. You set up promoted in-app purchases using App Store Connect, including their default display order and visibility settings. Use this API to override and customize their order and visibility. Overrides are per device. They can take effect after the user launches the app at least once.

You don’t instantiate this structure. To get a list of `Product.PromotionInfo` objects, call the static method updateProductOrder(byID:) with a list of product identifiers that represent your promoted in-app purchases. Then call currentOrder to get the list of `Product.PromotionInfo` objects. To change their order, call updateAll(_:) with the promoted in-app purchases listed in the desired order. To change the order using product identifiers, call updateProductOrder(byID:).

To prevent a promoted in-app purchase from appearing in the App Store on the device, there are two options:

- Hide the product by setting the visibility value to Product.PromotionInfo.Visibility.hidden and calling update(), or call updateProductVisibility(_:for:).

- Remove the product from the list by excluding it when you call updateAll(_:) or updateProductOrder(byID:).

To cancel your overrides and return to the default order and visibility, call updateAll(_:) or updateProductOrder(byID:) with an empty array.

For more information about promoting in-app purchases, see Supporting promoted In-App Purchases in your app.

## Topics

### Getting the product ID

let productID: Product.ID

The product identifier of the promoted in-app purchase.

### Managing promotion order

static func updateProductOrder(byID: some Collection&lt;String>) async throws

Sets the display order of promoted in-app purchases in the App Store, using product identifiers.

### Getting overridden order

static var currentOrder: [Product.PromotionInfo]

Gets the customized order of the promotion info objects the represent promoted products.

### Managing promotion visibility

var visibility: Product.PromotionInfo.Visibility

A value that indicates whether the promoted in-app purchase is visible or hidden on the user’s device.

enum Visibility

The visibility states for product promotion information.

static func updateProductVisibility(Product.PromotionInfo.Visibility, for: Product.ID) async throws

Updates a value that indicates whether a promoted in-app purchase appears in the App Store on the user’s device.

### Updating order and visibility

func update() async throws

Saves your changes to the promoted product’s visibility.

static func updateAll(some Collection&lt;Product.PromotionInfo>) async throws

Sets the order and visibility of all the promoted products and saves your changes.

## Relationships

### Conforms To

- Equatable

## See Also

### Promoted In-App Purchases

Supporting promoted In-App Purchases in your app

Display promoted In-App Purchases on your product page and handle purchases that users initiate on the App Store.

struct PurchaseIntent

An instance that emits purchase intents, which indicate that the customer initiated a purchase outside of your app, for your app to complete.

Testing promoted In-App Purchases

Test your In-App Purchases before making your app available in the App Store.

