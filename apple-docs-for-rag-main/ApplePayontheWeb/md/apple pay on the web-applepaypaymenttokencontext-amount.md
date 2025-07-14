

- Apple Pay on the Web
- ApplePayPaymentTokenContext
-  amount 

Instance Property

# amount

The amount to authorize for the payment token context.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString amount;
```

## Discussion

The sum of the amount of all the payment token contexts in a payment request must be less than or equal to the grand total amount of the enclosing payment request.

