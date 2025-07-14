

- StoreKit Test
-  FailableStoreKitAPI 

Protocol

# FailableStoreKitAPI

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol FailableStoreKitAPI : Sendable
```

## Topics

### Associated Types

associatedtype Failure : SKTestFailure

**Required**

### Type Properties

static var appStoreSync: StoreKitAppStoreSyncAPI

static var appTransaction: StoreKitAppTransactionAPI

static var loadProducts: StoreKitLoadProductsAPI

static var manageSubscriptions: StoreKitManageSubscriptionsAPI

static var offerCodeRedeem: StoreKitOfferCodeRedeemAPI

static var purchase: StoreKitPurchaseAPI

static var refundRequest: StoreKitRefundRequestAPI

static var subscriptionStatus: StoreKitSubscriptionStatusAPI

static var verification: StoreKitVerificationAPI

## Relationships

### Inherits From

- Sendable

### Conforming Types

- StoreKitAppStoreSyncAPI
- StoreKitAppTransactionAPI
- StoreKitLoadProductsAPI
- StoreKitManageSubscriptionsAPI
- StoreKitOfferCodeRedeemAPI
- StoreKitPurchaseAPI
- StoreKitRefundRequestAPI
- StoreKitSubscriptionStatusAPI
- StoreKitVerificationAPI

## See Also

### Protocols

protocol SKTestFailure

