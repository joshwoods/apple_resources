

- PassKit (Apple Pay and Wallet)
-  PKPaymentRequest 

Class

# PKPaymentRequest

An object that represents a request for payment, including details about payment-processing capabilities, the payment amount, and shipping information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
class PKPaymentRequest
```

## Overview

Use a PKPaymentRequest object to represent a merchant request for payment for goods or services. Your app creates a payment request as soon as a person taps the Apple Pay button to make a purchase. Tapping the Apple Pay button in your app initiates the payment request process. If your customers need to enter a discount code, choose a shipping method, or any other task, your app needs to ask for that information *before* they tap the Apple Pay button.

A payment request object contains information that describes the purchase, including information about the merchant, available payment networks, the payment summary, billing and shipping details, coupon codes, custom data, error messages, and more.

A typical payment request is for a one-time payment. To support different types of payment requests, include one of the following options in the payment request object:

| Payment type request | Property to set |
|----|----|
| Recurring payments | recurringPaymentRequest |
| Automatic reload payments | automaticReloadPaymentRequest |
| Deferred payments | deferredPaymentRequest |
| Indicating eligibility for Apple Pay Later | applePayLaterAvailability |
| Multiple payment tokens to support for multimerchant payments | multiTokenContexts |

Note

You can set only one optional payment request type on a payment request object.

### Request a recurring payment

Use the recurringPaymentRequest property to set up a recurring payment request using the PKRecurringPaymentRequest and PKRecurringPaymentSummaryItem classes. Recurring payments, such as subscriptions, can feature different payment intervals (for example, annually or monthly) and billing cycles, such as regular or trial.

### Request an automatic reload payment

Use the automaticReloadPaymentRequest property to set up an automatic reload payment request using the PKAutomaticReloadPaymentRequest and PKAutomaticReloadPaymentSummaryItem classes. You can set up automatic reload payments, such as store card top-ups, that feature a balance threshold and a reload amount. The card automatically reloads with the reload amount when the account drops below the balance threshold.

### Request a deferred payment

Use the deferredPaymentRequest property to set up a deferred payment request using the PKDeferredPaymentRequest class. Deferred payments include purchases, such as hotel bookings or pre-orders, where the card renders payment at a later date upon the receipt of goods or delivery of services.

### Set the Apple Pay Later mode

Use the applePayLaterAvailability property to indicate whether this payment request is eligible for Apple Pay Later. You can indicate that Apple Pay Later is unavailable for certain kinds of transactions, including subscriptions, items that require recurring payments or prohibited items, such as gift cards.

### Request multitoken or multimerchant payments

Use the multiTokenContexts property to request payment data for multimerchant payments with the PKPaymentTokenContext class. You can set up multitoken transactions to process and display payment requests with multiple merchants on one payment sheet, for example, a booking site where someone pays for a hotel, flight, and car rental from different merchants.

## Topics

### Selecting the payment networks

class func availableNetworks() -> [PKPaymentNetwork]

Returns the list of available payment methods that Apple Pay supports.

var supportedNetworks: [PKPaymentNetwork]

The payment methods that you support.

struct PKPaymentNetwork

A type that represents a payment method.

### Setting merchant information

struct MerchantCategoryCode

An optional four-digit struct, in ISO 18245 format, that represents the type of goods or service the merchant provides for the transaction.

var merchantIdentifier: String

Your merchant identifier.

var merchantCapabilities: PKMerchantCapability

A bit field of the payment-processing protocols and card types that you support.

struct PKMerchantCapability

Capabilities for processing payment.

### Setting currency and region information

var currencyCode: String

The three-letter ISO 4217 currency code that determines the currency the payment request uses.

var supportedCountries: Set&lt;String>?

A list of ISO 3166 country codes to limit payments to cards from specific countries or regions.

var countryCode: String

The merchant’s two-letter ISO 3166 country code.

### Setting the payment summary items

var paymentSummaryItems: [PKPaymentSummaryItem]

An array of payment summary item objects that summarize the amount of the payment.

class PKPaymentSummaryItem

An object that defines a summary item in a payment request, taxes, discounts, shipping, a grand total, and the like.

class PKRecurringPaymentSummaryItem

An object that defines a summary item for a payment that occurs repeatedly at a specified interval, such as a subscription.

class PKDeferredPaymentSummaryItem

An object that defines a summary item for a payment that occurs at a later date, such as a pre-order.

### Requesting recurring, automatic, and deferred payments

var recurringPaymentRequest: PKRecurringPaymentRequest?

An optional request to set up a recurring payment, typically a subscription.

class PKRecurringPaymentRequest

A class that represents a request to set up a recurring payment, typically a subscription.

var automaticReloadPaymentRequest: PKAutomaticReloadPaymentRequest?

An optional request to set up an automatic reload payment, such as a store card top-up.

class PKAutomaticReloadPaymentRequest

A class that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

var deferredPaymentRequest: PKDeferredPaymentRequest?

A request to set up a deferred payment, such as a hotel booking or a pre-order.

class PKDeferredPaymentRequest

An object that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

### Requesting multitoken or multimerchant payments

var multiTokenContexts: [PKPaymentTokenContext]

An array of payment token contexts to request multiple payment tokens with one payment token per context.

class PKPaymentTokenContext

A class that defines the context for a single payment token in a payment request for multimerchant payments.

### Requesting billing and shipping contact fields

var requiredBillingContactFields: Set&lt;PKContactField>

A list of fields that you need for a billing contact to process the transaction.

var requiredShippingContactFields: Set&lt;PKContactField>

A list of fields that you need for a shipping contact to process the transaction.

struct PKContactField

The fields that describe a contact.

### Providing known contact information

var billingContact: PKContact?

A prepopulated billing address.

var shippingContact: PKContact?

A prepopulated shipping address.

class PKContact

An object that encapsulates contact information needed for billing and shipping.

### Setting the shipping methods and types

Displaying a Read-Only Pickup Address

Configure a payment request to display a read-only pickup address on the payment sheet.

var shippingMethods: [PKShippingMethod]?

An array of shipping method objects that describe the supported shipping methods.

class PKShippingMethod

An object that defines a shipping method for delivering physical goods.

var shippingType: PKShippingType

The type of shipping the request uses.

var shippingContactEditingMode: PKShippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

enum PKShippingType

A complete list of valid shipping types.

enum PKShippingContactEditingMode

Constants that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

### Working with coupon codes

var couponCode: String?

The initial coupon code for the payment request.

var supportsCouponCode: Bool

A Boolean value that determines whether the payment sheet displays the coupon code field.

### Adding custom data

var applicationData: Data?

Application-specific data or state.

### Providing error information

Create common payment errors using these simple convenience functions.

class func paymentBillingAddressInvalidError(withKey: String, localizedDescription: String?) -> any Error

Creates a billing address error with the supplied key and user-facing error message.

class func paymentContactInvalidError(withContactField: PKContactField, localizedDescription: String?) -> any Error

Creates a contact error with the supplied field and user-facing error message.

class func paymentShippingAddressInvalidError(withKey: String, localizedDescription: String?) -> any Error

Creates a shipping address error with the supplied key and user-facing error message.

class func paymentShippingAddressUnserviceableError(withLocalizedDescription: String?) -> any Error

Creates an error for an unserviceable address, with the supplied user-facing error message.

static func paymentCouponCodeInvalidError(localizedDescription: String?) -> any Error

Returns an error object that indicates an invalid coupon.

static func paymentCouponCodeExpiredError(localizedDescription: String?) -> any Error

Returns an error object that indicates an expired coupon.

### Deprecated

static var enabled: PKShippingContactEditingMode

All fields of the shipping contact on the payment sheet are editable by the user.

Deprecated

var requiredBillingAddressFields: PKAddressField

A bit field of billing address fields that you need in order to process the transaction.

Deprecated

var requiredShippingAddressFields: PKAddressField

A bit field of shipping address fields that you need in order to process the transaction.

Deprecated

struct PKAddressField

Billing or shipping address fields.

Deprecated

var billingAddress: ABRecord?

A prepopulated billing address.

Deprecated

var shippingAddress: ABRecord?

A prepopulated shipping address.

Deprecated

### Enumerations

enum ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

### Instance Properties

var applePayLaterAvailability: PKPaymentRequest.ApplePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

Deprecated

var merchantCategoryCode: PKPaymentRequest.MerchantCategoryCode?

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

## See Also

### Payment requests

class PKRecurringPaymentRequest

A class that represents a request to set up a recurring payment, typically a subscription.

class PKAutomaticReloadPaymentRequest

A class that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

class PKDeferredPaymentRequest

An object that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

class PKPaymentTokenContext

A class that defines the context for a single payment token in a payment request for multimerchant payments.

