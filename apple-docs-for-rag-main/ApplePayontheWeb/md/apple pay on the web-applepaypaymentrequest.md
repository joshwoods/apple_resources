

- Apple Pay on the Web
-  ApplePayPaymentRequest 

Structure

# ApplePayPaymentRequest

A request for payment, which includes information about payment-processing capabilities, the payment amount, and shipping information.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayPaymentRequest {
 required sequence  merchantCapabilities;
 required sequence  supportedNetworks;
 required DOMString countryCode;
 sequence  requiredBillingContactFields;
 ApplePayPaymentContact billingContact;
 sequence  requiredShippingContactFields;
 ApplePayPaymentContact shippingContact;
 DOMString applicationData;
 sequence  supportedCountries;
 boolean supportsCouponCode;
 DOMString couponCode;
 ApplePayShippingContactEditingMode shippingContactEditingMode;
 required ApplePayLineItem total;
 sequence  lineItems;
 required DOMString currencyCode;
 ApplePayShippingType shippingType;
 sequence  shippingMethods;
 sequence  multiTokenContexts;
 ApplePayAutomaticReloadPaymentRequest automaticReloadPaymentRequest;
 ApplePayRecurringPaymentRequest recurringPaymentRequest;
 ApplePayDeferredPaymentRequest deferredPaymentRequest;
};
```

## Mentioned in 

Creating an Apple Pay Session

Apple Pay on the Web Version 12 Release Notes

Apple Pay on the Web Version 4 Release Notes

Apple Pay on the Web Version 14 Release Notes

Apple Pay on the Web Version 3 Release Notes

## Overview

Use an ApplePayPaymentRequest dictionary to represent a merchant request for payment for goods or services. Your website creates a payment request as soon as the user taps the Apple Pay button to make a purchase.

A payment request contains information that describes the purchase, such as the merchant information, supported payment networks, and the line items, including the total, the currency code, the billing and shipping contact, and more.

A typical payment request is for a one-time payment. To support different types of payment requests, provide one of the following options in the payment request:

- A recurringPaymentRequest object to request a recurring payment. Recurring payments, such as subscriptions, can feature different payment intervals (for example, annually or monthly), and either regular or trial billing cycles.

- An automaticReloadPaymentRequest object to set up automatic reload payments. Automatic reload payments, such as store card top-ups, feature a balance threshold and a reload amount. The card automatically reloads with the reload amount when the account drops below the balance threshold.

- Use the deferredPaymentRequest property to set up a deferred payment request using the ApplePayDeferredPaymentRequest class. Deferred payments include purchases, such as hotel bookings or pre-orders, where the card renders payment at a later date upon the receipt of goods or delivery of services.

- Use the applePayLaterAvailability property to indicate whether this payment request is eligible for Apple Pay Later. You can indicate that Apple Pay Later is unavailable for certain kinds of transactions, including subscriptions, items that require recurring payments or prohibited items, such as gift cards.

- A multiTokenContexts sequence to request multiple payment tokens to support multimerchant payments. Set up multitoken transactions to process and display payment requests with multiple merchants on one payment sheet, for example, a booking site where a user pays for a hotel, flight, and car rental from different merchants.

Note

You can set only one of these optional payment request type properties on a payment request object.

For recurring payments and automatic reload payments, you can optionally set up merchant token life-cycle notifications for the request. For more information, see Apple Pay Merchant Token Management API.

## Topics

### Setting the total and summary line items

total

A line item that represents the total for the payment.

lineItems

A set of line items that explain recurring payments and additional charges and discounts.

ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

ApplePayLineItemType

A type that indicates whether a line item is final or pending.

### Requesting recurring payments

recurringPaymentRequest

A property that requests a recurring payment, typically a subscription.

ApplePayRecurringPaymentRequest

A dictionary that represents a request to set up a recurring payment, typically a subscription.

### Requesting automatic reload payments

automaticReloadPaymentRequest

A property that requests an automatic reload payment, such as a store card top-up.

ApplePayAutomaticReloadPaymentRequest

A dictionary that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

### Requesting deferred payments

deferredPaymentRequest

A property that requests a deferred payment, such as a hotel booking or a pre-order.

### Requesting multitoken or multimerchant payments

multiTokenContexts

An array of payment token contexts that requests multiple payment tokens to support a multimerchant payment.

ApplePayPaymentTokenContext

A dictionary that defines the context for a single payment token in a payment request for multimerchant payments.

### Working with transaction information

countryCode

The merchant’s two-letter ISO 3166 country code.

currencyCode

The three-letter ISO 4217 currency code for the payment.

merchantCapabilities

An array of the payment capabilities that the merchant supports, such as credit or debit.

shippingMethods

The list of shipping methods available for a payment request.

shippingType

An optional value that indicates how to ship purchased items.

supportedCountries

A list of two-letter country codes for limiting payment to cards from specific countries or regions.

supportedNetworks

The payment networks the merchant supports.

ApplePayMerchantCapability

The payment capabilities the merchant supports.

ApplePayShippingMethod

A dictionary that describes the shipping method for delivering physical goods.

ApplePayShippingType

A type that indicates how to ship purchased items.

### Requesting billing and shipping contact information

requiredBillingContactFields

The fields of billing information the user must provide to process the transaction.

requiredShippingContactFields

The fields of shipping information the user must provide to fulfill the order.

shippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

ApplePayContactField

Field names for requesting contact information in a payment request.

ApplePayShippingContactEditingMode

Values that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

### Providing known contact information

billingContact

Billing contact information for the user.

shippingContact

Shipping contact information for the user.

ApplePayPaymentContact

Contact information fields to use for billing and shipping contact information.

### Working with coupon codes

couponCode

The initial coupon code for the payment request.

supportsCouponCode

A Boolean value that determines whether the payment sheet displays the coupon code field.

### Adding custom data

applicationData

A Base64-encoded string for application-specific data.

## See Also

### Apple Pay payment request

ApplePayDeferredPaymentRequest

A dictionary that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

