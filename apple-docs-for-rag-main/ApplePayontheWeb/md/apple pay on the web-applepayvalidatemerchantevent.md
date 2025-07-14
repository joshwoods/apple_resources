

- Apple Pay on the Web
-  ApplePayValidateMerchantEvent 

Class

# ApplePayValidateMerchantEvent

An event object that contains the validation URL.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
interface ApplePayValidateMerchantEvent
```

## Mentioned in 

Providing Merchant Validation

## Overview

The event handler onvalidatemerchant receives this event object when the payment sheet is displayed.

## Topics

### Accessing the Merchant Validation Event Attributes

validationURL

The URL your server must use to validate itself and obtain a merchant session object.

## See Also

### Getting merchant validation

begin

Begins the merchant validation process.

onvalidatemerchant

An event handler the system calls when it displays the payment sheet.

completeMerchantValidation

Completes the validation for a merchant session.

