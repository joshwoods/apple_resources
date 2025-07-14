

- Apple Pay on the Web
-  ApplePayPaymentTokenContext 

Structure

# ApplePayPaymentTokenContext

A dictionary that defines the context for a single payment token in a payment request for multimerchant payments.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayPaymentTokenContext {
 required DOMString merchantIdentifier;
 required DOMString externalIdentifier;
 required DOMString merchantName;
 DOMString merchantDomain;
 required DOMString amount;
};
```

## Overview

Important

You must include the multiTokenContexts array in the ApplePayPaymentRequest object to request multimerchant payments.

Use ApplePayPaymentTokenContext to authorize a payment amount for each payment token in a multimerchant payment request. To enable multiple merchants for a transaction, use one ApplePayPaymentTokenContext object for each merchant.

You can optionally associate each payment token with the merchant’s top-level domain.

## Topics

### Specifying the merchant

merchantIdentifier

The Apply Pay merchant identifier.

merchantName

The merchant’s display name that the Apple Pay server associates with the payment token.

merchantDomain

The merchant’s top-level domain that the Apple Pay server associates with the payment token.

externalIdentifier

An external identifier for the merchant.

### Indicating a payment amount

amount

The amount to authorize for the payment token context.

## See Also

### Requesting multitoken or multimerchant payments

multiTokenContexts

An array of payment token contexts that requests multiple payment tokens to support a multimerchant payment.

