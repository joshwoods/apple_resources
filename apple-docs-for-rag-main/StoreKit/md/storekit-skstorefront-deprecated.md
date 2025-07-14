

- StoreKit
-  SKStorefront Deprecated

Class

# SKStorefront

An object containing the location and unique identifier of an Apple App Store storefront.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0DeprecatedtvOS 13.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKStorefront
```

Deprecated

Use Storefront instead.

## Mentioned in 

Testing In-App Purchases with sandbox

## Overview

In-app products you create through App Store Connect are available for sale in every region with an App Store. You can use the storefront information to determine the customer’s region, and offer in-app products suitable for that region. StoreKit exposes SKStorefront storefront information as a read-only property in SKPaymentQueue.

You must maintain your own list of product identifiers and the storefronts in which you want to make them available.

Note

Don’t save the storefront information with your customer information; storefront information can change at any time. Always get the storefront identifier immediately before you display product information or availability to the customer in your app. Storefront information may not be used to develop or enhance a customer profile, or track customers for advertising or marketing purposes.

### Show Products Based on the Current Storefront

The following example function `shouldShow` returns `false` if your product isn’t suitable for the given storefront. You must create your own list of products available by storefront, referred to as `myProducts` below:

```
func shouldShow(_ productIdentifier: String, in storefront: SKStorefront) -> Bool {
    var shouldShow = true

    // myProducts is a dictionary representing your own metadata for products,
    // keyed on an SKProduct.productIdentifier.
    if let myProduct = myProducts[productIdentifier] {
        shouldShow = myProduct.countryCodes.contains(storefront.countryCode)
    }
    return shouldShow
}
```

The following code listing requests information for products that you wish to display based on the device’s storefront. It uses the `shouldShow` function defined above.

```
func fetchProductInfo() {
    var identifiers = Set()
    if let storefront = SKPaymentQueue.default().storefront {
        for (identifier, _) in myProducts {
            if shouldShow(identifier, in: storefront) {
                identifiers.insert(identifier)
            }
        }
        let request = SKProductsRequest(productIdentifiers: identifiers)
        request.delegate = self
        request.start()
    }
}
```

### Listen for Storefront Changes

The storefront value can change at any time. To listen for changes in this value, implement the paymentQueueDidChangeStorefront(_:) method. The `shouldShow` function is defined in Show Products Based on the Current Storefront. Refresh the list of your available products when the storefront changes, as shown below:

```
func paymentQueueDidChangeStorefront(_ queue: SKPaymentQueue) {
    if let storefront = queue.storefront {
        // Refresh the displayed products based on the new storefront.
        for product in storeProducts {
            if shouldShow(product.productIdentifier, in: storefront) {
                // Display this product in your store UI.
         }
      }
   }
}
```

### Respond to Storefront Changes

The current storefront can change at any time, including during a transaction. The following code listing determines whether the transaction should continue in the updated storefront. Your delegate’s paymentQueue(_:shouldContinue:in:) method must return quickly, before the call times out. The `shouldShow` function is defined in Show Products Based on the Current Storefront.

```
SKPaymentQueue.default().delegate = self  // Set your object as the SKPaymentQueue delegate.

func paymentQueue(_ paymentQueue: SKPaymentQueue,
                  shouldContinue transaction: SKPaymentTransaction,
                  in newStorefront: SKStorefront) -> Bool {
    return shouldShow(transaction.payment.productIdentifier, in: newStorefront)
}
```

If the product isn’t available in the updated storefront, the transaction fails with the error SKError.Code.storeProductNotAvailable. Handle this error in your paymentQueue(_:updatedTransactions:) method by displaying an alert to let the customer know why the app can’t complete the transaction, as shown below:

```
func paymentQueue(_ queue: SKPaymentQueue,
                  updatedTransactions transactions: [SKPaymentTransaction]) {
    for transaction in transactions {
        if let transactionError = transaction.error as NSError?,
            transactionError.domain == SKErrorDomain
            && transactionError.code == SKError.storeProductNotAvailable.rawValue {
            // Show an alert.
        }
    }
}
```

### Change the App Store Country or Region in the Sandbox Environment

When you change the App Store Country or Region in App Store Connect for a Sandbox Apple ID, it changes the storefront in your app. Change the region to test in-app purchases for different regions in your app. For more information about changing the App Store Country or Region in App Store Connect, see Test in-app purchases.

Important

To successfully activate a storefront after you change the region in App Store Connect, sign out of the Sandbox Apple ID account on the device and sign back in.

## Topics

### Identifying the Storefront

var countryCode: String

The three-letter code representing the country or region associated with the App Store storefront.

var identifier: String

A value defined by Apple that uniquely identifies an App Store storefront.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

