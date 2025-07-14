

- Apple Pay on the Web
-  ApplePayPaymentTiming 

Enumeration

# ApplePayPaymentTiming

A type that indicates the time a payment occurs in a transaction.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum ApplePayPaymentTiming
```

## Mentioned in 

Apple Pay on the Web Version 14 Release Notes

## Overview

The following are the payment timing values:

`"immediate"`  
A value that specifies that the payment occurs when the transaction is complete.

`"recurring"`  
A value that specifies that the payment occurs on a regular basis.

`"deferred"`  
A value that specifies that the payment occurs in the future.

`"automaticReload"`  
A value that specifies that the payment occurs automatically when the account falls below the automaticReloadPaymentThresholdAmount amount.

## Topics

### Enumeration Cases

automaticReload

deferred

immediate

recurring

## See Also

### Configuring payment timing

paymentTiming

The time that the payment occurs as part of a successful transaction.

