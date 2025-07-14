

- Apple Pay on the Web
-  ApplePayPaymentPassActivationState 

Enumeration

# ApplePayPaymentPassActivationState

Payment pass activation states.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum ApplePayPaymentPassActivationState
```

## Overview

Use one of the following values for the activation state:

`activated`  
Active and ready to be used for payment.

`requiresActivation`  
Not active but may be activated by the issuer.

`activating`  
Not ready for use but activation is in progress.

`suspended`  
Not active and can’t be activated.

`deactivated`  
Not active because the issuer has disabled the account associated with the device.

## Topics

### Enumeration Cases

activated

activating

deactivated

requiresActivation

suspended

## See Also

### Activation State

activationState

The activation state of the pass.

