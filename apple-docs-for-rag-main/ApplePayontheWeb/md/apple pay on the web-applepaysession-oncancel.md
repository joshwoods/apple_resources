

- Apple Pay on the Web
- ApplePaySession
-  oncancel 

Instance Property

# oncancel

An event handler that is automatically called when the payment UI is dismissed.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute EventHandler oncancel;
```

## Discussion

This function can be called even after an onpaymentauthorized event has been dispatched. Both the user and the web page can dismiss the payment sheet and abandon the transaction.

## See Also

### Ending the session

abort

Aborts the current Apple Pay session.

