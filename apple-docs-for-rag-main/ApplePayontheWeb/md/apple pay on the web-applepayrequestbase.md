

- Apple Pay on the Web
-  ApplePayRequestBase 

Structure

# ApplePayRequestBase

A dictionary that defines basic payment and contact information that the Apple Pay payment request object uses for the W3C Payment Request API.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayRequestBase {
 sequence  features;
 required sequence  merchantCapabilities;
 required sequence  supportedNetworks;
 required DOMString countryCode;
 sequence  requiredBillingContactFields;
 ApplePayPaymentContact billingContact;
 sequence  requiredShippingContactFields;
 ApplePayPaymentContact shippingContact;
 DOMString applicationData;
 sequence  supportedCountries;
 ApplePayInstallmentConfiguration installmentConfiguration;
 boolean supportsCouponCode;
 DOMString couponCode;
 ApplePayShippingContactEditingMode shippingContactEditingMode;
 ApplePayLaterAvailability applePayLaterAvailability;
};
```

## Topics

### Setting the transaction information

countryCode

The merchant’s two-letter ISO-3166 country code.

merchantCapabilities

An array of the payment capabilities that the merchant supports, such as credit or debit card payments.

supportedNetworks

The payment networks the merchant provides to their customers.

supportedCountries

A list of two-letter country codes for limiting payment to credit cards from specific countries or regions.

### Managing coupon codes

couponCode

The initial coupon code for the payment request.

supportsCouponCode

A Boolean value that determines whether the payment sheet displays the coupon code field.

### Billing and shipping information

requiredBillingContactFields

A list of fields use for processing the transaction, including the name, address, and other information associated with the payment method.

requiredShippingContactFields

A list of fields used for processing the transaction, including the recipient’s name, mailing address, and other contact details.

### Setting contact information

billingContact

A prepopulated billing address.

shippingContact

The customer’s address, used for sending products or services for to the person.

shippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

### Adding custom data

applicationData

Application-specific data or state you can add to support your app.

### Adding an installment configuration

installmentConfiguration

### Adding features

features

### Deprecated

ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

applePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

Deprecated

## See Also

### Payment request

Setting up the payment request API to accept Apple Pay

Support payments using Apple Pay on your website.

ApplePayRequest

A dictionary that defines the Apple Pay payment request object to use for the W3C Payment Request API.

ApplePayModifier

A dictionary that defines the Apple Pay modifiers for a payment type in the W3C Payment Request API.

ApplePayPaymentCompleteDetails

