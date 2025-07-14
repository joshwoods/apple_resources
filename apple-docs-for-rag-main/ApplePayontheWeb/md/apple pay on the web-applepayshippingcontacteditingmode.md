

- Apple Pay on the Web
-  ApplePayShippingContactEditingMode 

Enumeration

# ApplePayShippingContactEditingMode

Values that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum ApplePayShippingContactEditingMode
```

## Overview

The values for the contact editing mode:

`“available”`  
The user can edit the shipping contact on the payment sheet.

“`enabled`” (deprecated)  
The user can edit the shipping contact on the payment sheet.

`“storePickup”`  
The user can’t edit the shipping contact on the payment sheet.

Important

Previous versions of the Apple Pay JS API accepted `enabled` rather than `available` as a parameter for the `ApplePayShippingContactEditingMode`. Developers should upgrade their code to use `available`.\`\`

## Topics

### Enumeration Cases

enabled

storePickup

## See Also

### Requesting billing and shipping contact information

requiredBillingContactFields

The fields of billing information the user must provide to process the transaction.

requiredShippingContactFields

The fields of shipping information the user must provide to fulfill the order.

shippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

ApplePayContactField

Field names for requesting contact information in a payment request.

