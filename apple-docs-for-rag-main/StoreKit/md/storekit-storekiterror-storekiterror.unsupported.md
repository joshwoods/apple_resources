

- StoreKit
- StoreKitError
-  StoreKitError.unsupported 

Case

# StoreKitError.unsupported

The operation doesn’t support this product.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
case unsupported
```

## Discussion

The system surfaces this error when the type that originates the request doesn’t support the operation. For example, initializing an AdvancedCommerceProduct using the product ID of an in-app purchase that isn’t registered as a generic SKU in App Store Connect.

## See Also

### StoreKit Error Codes

case networkError(URLError)

A network error occurred.

case systemError(any Error)

A system error occurred.

case userCancelled

The user canceled.

case notAvailableInStorefront

The function isn’t available on devices configured for this storefront.

case notEntitled

The app doesn’t have the appropriate entitlements to use the functionality.

case unknown

An unknown error occurred.

