

- Apple Pay on the Web
-  ApplePayShippingMethod 

Structure

# ApplePayShippingMethod

A dictionary that describes the shipping method for delivering physical goods.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayShippingMethod {
 required DOMString label;
 required DOMString detail;
 required DOMString amount;
 required DOMString identifier;
 ApplePayDateComponentsRange dateComponentsRange;
};
```

## Mentioned in 

Apple Pay on the Web Version 12 Release Notes

## Overview

The Apple Pay sheet displays all the properties of a shipping method except `identifier`. The following listing is an example of a shipping method that shows free shipping.

```
{    
    "label": "Free Shipping",
    "detail": "Arrives in 5 to 7 days",
    "amount": "0.00",
    "identifier": "FreeShip"
}

```

## Topics

### Working with shipping method properties

label

A short description of the shipping method.

detail

Additional description of the shipping method.

dateComponentsRange

The expected range of dates for shipping or picking up an item.

identifier

A client-defined value used to identify this shipping method.

amount

The nonnegative cost associated with this shipping method.

ApplePayDateComponentsRange

A dictionary that specifies the start and end dates for a range of time.

## See Also

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

ApplePayShippingType

A type that indicates how to ship purchased items.

