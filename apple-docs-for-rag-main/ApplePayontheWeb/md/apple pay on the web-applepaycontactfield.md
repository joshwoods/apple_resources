

- Apple Pay on the Web
-  ApplePayContactField 

Enumeration

# ApplePayContactField

Field names for requesting contact information in a payment request.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum ApplePayContactField
```

## Mentioned in 

Apple Pay on the Web Version 3 Release Notes

## Overview

Contact field values (available in all versions of the API):

`"email"`

`"name"`

`"phone"`

`"postalAddress"`

Contact field values available starting in API version 3:\`\`

`"phoneticName"`

## Topics

### Enumeration Cases

email

name

phone

phoneticName

postalAddress

## See Also

### Requesting billing and shipping contact information

requiredBillingContactFields

The fields of billing information the user must provide to process the transaction.

requiredShippingContactFields

The fields of shipping information the user must provide to fulfill the order.

shippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

ApplePayShippingContactEditingMode

Values that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

