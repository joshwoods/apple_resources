

- Apple Pay on the Web
- ApplePaySession
-  abort 

Instance Method

# abort

Aborts the current Apple Pay session.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
undefined abort();
```

## Discussion

Dismisses the payment sheet and ends the Apple Pay session without completing a transaction. Only the web page can call abort.

## See Also

### Ending the session

oncancel

An event handler that is automatically called when the payment UI is dismissed.

