

- PassKit (Apple Pay and Wallet)
-  PKPaymentRequestUpdate 

Class

# PKPaymentRequestUpdate

The base class for updating the payment request after the user makes changes on the payment sheet.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class PKPaymentRequestUpdate
```

## Topics

### Creating a payment request update

init(paymentSummaryItems: [PKPaymentSummaryItem])

Creates a payment request update with the specified payment summary items.

### Updating authorization status

var status: PKPaymentAuthorizationStatus

The status of the payment request that indicates whether authorization succeeds or fails.

enum PKPaymentAuthorizationStatus

General success and failure status for payment authorization.

### Updating summary items

var paymentSummaryItems: [PKPaymentSummaryItem]

The list of payment summary items for the instance.

class PKPaymentSummaryItem

An object that defines a summary item in a payment request, taxes, discounts, shipping, a grand total, and the like.

### Updating shipping methods

var shippingMethods: [PKShippingMethod]

The list of shipping methods available for a payment request.

### Updating automatic reload payments

var automaticReloadPaymentRequest: PKAutomaticReloadPaymentRequest?

The automatic reload payment request to update the payment request with.

### Updating multitoken or multimerchant payments

var multiTokenContexts: [PKPaymentTokenContext]?

An optional array of payment token contexts to request multiple payment tokens with one payment token per context.

### Updating recurring payments

var recurringPaymentRequest: PKRecurringPaymentRequest?

The recurring payment request to update the payment request with.

### Setting up a deferred payment request

var deferredPaymentRequest: PKDeferredPaymentRequest?

The deferred payment request to update the payment request with.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PKPaymentRequestCouponCodeUpdate
- PKPaymentRequestPaymentMethodUpdate
- PKPaymentRequestShippingContactUpdate
- PKPaymentRequestShippingMethodUpdate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Payment sheet updates

class PKPaymentRequestMerchantSessionUpdate

An object that updates a payment request with a merchant validation.

class PKPaymentRequestPaymentMethodUpdate

An object that updates the payment request after the payment method changes.

class PKPaymentRequestShippingContactUpdate

An object that updates the payment request after the shipping contact information changes.

class PKPaymentRequestShippingMethodUpdate

An object that updates the payment request after the shipping method changed.

class PKPaymentRequestCouponCodeUpdate

An object that updates the payment request after the coupon code changes.

