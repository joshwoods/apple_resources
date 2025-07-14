

- Apple Pay on the Web
- ApplePaySession
-  begin 

Instance Method

# begin

Begins the merchant validation process.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
undefined begin();
```

## Mentioned in 

Creating an Apple Pay Session

## Discussion

When this method is called, the payment sheet is presented and the merchant validation process is initiated.

## See Also

### Getting merchant validation

onvalidatemerchant

An event handler the system calls when it displays the payment sheet.

completeMerchantValidation

Completes the validation for a merchant session.

ApplePayValidateMerchantEvent

An event object that contains the validation URL.

