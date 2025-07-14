

- StoreKit
-  StoreKitError 

Enumeration

# StoreKitError

StoreKit In-App Purchase error codes.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum StoreKitError
```

## Topics

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

case unsupported

The operation doesn’t support this product.

## Relationships

### Conforms To

- Copyable
- Error
- LocalizedError
- Sendable

