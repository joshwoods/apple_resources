

- StoreKit
- In-App Purchase
- Product.SubscriptionInfo.RenewalInfo
-  Managing Price Increases for Auto-Renewable Subscriptions 

Article

# Managing Price Increases for Auto-Renewable Subscriptions

Identify the price increase status for auto-renewable subscriptions in your app and on your server.

## Overview

If you increase the price of an auto-renewable subscription in App Store Connect, the priceIncreaseStatus in the renewalInfo object indicates if the subscription is subject to the price increase. Auto-renewable subscriptions have two types of price increases: those that require customer consent, and those that don’t require customer consent.

For price increases that require customer consent, look for the following status values in your app:

| Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus.noIncreasePending | Indicates there’s no price increase for this auto-renewable subscription. |
|----|----|
| Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus.pending | Indicates there’s a pending price increase for the auto-renewable subscription that requires customer consent, and the customer hasn’t yet consented.  If the customer doesn’t consent, the auto-renewable subscription expires at the end of the billing cycle. When it expires, your app gets a status update in updates with an expirationReason of didNotConsentToPriceIncrease. |
| Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus.agreed | Indicates that the customer consented to a price increase for the auto-renewable subscription. |

For price increases that don’t require customer consent, look for the following status values in your app:

| Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus.noIncreasePending | Doesn’t apply. |
|----|----|
| Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus.pending | Doesn’t apply. |
| Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus.agreed | Indicates that the App Store informed the customer of the price increase for the auto-renewable subscription, and the subscription is subject to the price increase.  If the customer cancels the auto-renewable subscription, your app gets a status update in updates with an expirationReason of autoRenewDisabled. |

For more information about managing subscription prices in App Store Connect, see Managing Prices.

### Receive Notifications for Price Increase Status Events

If you’ve enabled App Store Server Notifications V2, your server receives notifications for events related to auto-renewable subscription price increases.

For auto-renewable subscription price increases that require customer consent, look for the following notifications:

| Notification type | Subtype | Description |
|----|----|----|
| `PRICE_INCREASE`  | `PENDING` | Indicates that the App Store informed the customer of the price increase for the auto-renewable subscription, and the customer hasn’t yet responded. |
| `PRICE_INCREASE` | `ACCEPTED` | Indicates that the customer consented to the price increase for the auto-renewable subscription. |
| `EXPIRED` | `PRICE_INCREASE` | Indicates that the auto-renewable subscription expired because the customer didn’t consent to the price increase, and allowed the subscription to expire. |
| `EXPIRED` | `VOLUNTARY` | Indicates that the customer voluntarily canceled the auto-renewable subscription. (Note: This notification type and subtype isn’t specific to price increases.) |

For auto-renewable subscription price increases that don’t require customer consent, look for the following notifications:

| Notification type | Subtype | Description |
|----|----|----|
| `PRICE_INCREASE` | `ACCEPTED` | Indicates that the App Store informed the customer of the auto-renewable subscription price increase, and the subscription is subject to the price increase. |
| `EXPIRED` | `VOLUNTARY` | Indicates that the customer voluntarily canceled the auto-renewable subscription. (Note: This notification type and subtype isn’t specific to price increases.) |

For more information about App Store Server Notifications, see Enabling App Store Server Notifications. For more information about notification types and subtypes, see notificationType and subtype.

## See Also

### Getting the price increase status

let priceIncreaseStatus: Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus

The status that indicates whether the auto-renewable subscription is subject to a price increase.

enum PriceIncreaseStatus

Status values that indicate whether an auto-renewable subscription is subject to a price increase.

