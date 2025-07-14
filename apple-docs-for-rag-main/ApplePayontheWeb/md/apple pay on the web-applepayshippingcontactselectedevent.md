

- Apple Pay on the Web
-  ApplePayShippingContactSelectedEvent 

Class

# ApplePayShippingContactSelectedEvent

An event object that contains the shipping address the user selects.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
interface ApplePayShippingContactSelectedEvent
```

## Overview

The event handler onshippingcontactselected receives this event object when the user selects a shipping contact.

## Topics

### Shipping Contact Properties

shippingContact

The shipping address selected by the user.

## See Also

### Handling shipping contact updates

onshippingcontactselected

An event handler to call when the user selects a shipping contact in the payment sheet.

completeShippingContactSelection

Completes the selection of a shipping contact with an update.

ApplePayShippingContactUpdate

Updated transaction details that result from a change in shipping contact, including any errors.

