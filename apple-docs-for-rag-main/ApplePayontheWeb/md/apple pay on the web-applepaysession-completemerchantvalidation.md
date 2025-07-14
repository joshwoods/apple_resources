

- Apple Pay on the Web
- ApplePaySession
-  completeMerchantValidation 

Instance Method

# completeMerchantValidation

Completes the validation for a merchant session.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
undefined completeMerchantValidation(
 any merchantSession
);
```

## Parameters 

`merchantSession`  

An opaque message session object, received from the Apple Pay server.

## Mentioned in 

Requesting an Apple Pay payment session

Providing Merchant Validation

## Discussion

Your server receives the merchant session object when it calls the `Payment Session` endpoint as described in Providing Merchant Validation.

You must pass the valid merchant session object to the completeMerchantValidation method to enable the user to authorize a transaction.

The guidelines for working with a merchant session are:

- Request a new merchant session object for each transaction. You can only use a merchant session object a single time.

- The merchant session object expires five minutes after it is created.

- Never request the merchant session from the client. The request must be sent from your server.

## See Also

### Getting merchant validation

begin

Begins the merchant validation process.

onvalidatemerchant

An event handler the system calls when it displays the payment sheet.

ApplePayValidateMerchantEvent

An event object that contains the validation URL.

