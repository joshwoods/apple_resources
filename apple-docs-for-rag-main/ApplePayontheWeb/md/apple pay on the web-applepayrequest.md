

- Apple Pay on the Web
-  ApplePayRequest 

Structure

# ApplePayRequest

A dictionary that defines the Apple Pay payment request object to use for the W3C Payment Request API.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayRequest {
 required long version;
 required DOMString merchantIdentifier;
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
};
```

## Mentioned in 

Apple Pay on the Web Version 12 Release Notes

Setting up the payment request API to accept Apple Pay

Apple Pay on the Web Version 6 Release Notes

## Overview

The dictionary contains the supported Apple Pay properties for the `data` object of the `PaymentMethodData` dictionary in the Payment Request API.

For more information on `PaymentMethodData`, see the W3C Payment Request API specification.

## Topics

### Identifier and version information

merchantIdentifier

The merchant identifier you registered with Apple for use with Apple Pay.

version

The Apple Pay version supported on your website.

### Transaction information

countryCode

The merchant’s two-letter ISO 3166 country code.

merchantCapabilities

An array of the payment capabilities the merchant supports, such as credit or debit.

supportedNetworks

The payment networks the merchant supports.

supportedCountries

A list of two-letter country codes for limiting payment to cards from specific countries or regions.

### Setting the Apple Pay Later mode

applePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

Deprecated

ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

### Coupon codes

couponCode

The initial coupon code for the payment request.

supportsCouponCode

A Boolean value that determines whether the payment sheet displays the coupon code field.

### Requesting billing and shipping contact information

requiredBillingContactFields

The fields of billing information the user must provide to process the transaction.

requiredShippingContactFields

The fields of shipping information the user must provide to fulfill the order.

### Known contact information

billingContact

The customer’s billing contact information.

shippingContact

The customer’s shipping contact information.

shippingContactEditingMode

A value that indicates if the shipping mode prevents the user editing the shipping address.

ApplePayPaymentContact

Contact information fields to use for billing and shipping contact information.

ApplePayShippingContactEditingMode

Values that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

### Respond to payment request change events

PaymentMethodChangeEvent

The Apple Pay extensions to the Payment Request payment change event.

ApplePayCouponCodeDetails

A dictionary that contains the updated coupon code.

### Custom data

applicationData

A Base64-encoded string used to contain your application-specific data.

## See Also

### Payment request

Setting up the payment request API to accept Apple Pay

Support payments using Apple Pay on your website.

ApplePayRequestBase

A dictionary that defines basic payment and contact information that the Apple Pay payment request object uses for the W3C Payment Request API.

ApplePayModifier

A dictionary that defines the Apple Pay modifiers for a payment type in the W3C Payment Request API.

ApplePayPaymentCompleteDetails

