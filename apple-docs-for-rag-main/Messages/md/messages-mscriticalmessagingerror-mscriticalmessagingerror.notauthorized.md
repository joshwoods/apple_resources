

- Messages
- MSCriticalMessagingError
-  MSCriticalMessagingError.notAuthorized 

Case

# MSCriticalMessagingError.notAuthorized

The operation isn’t authorized.

iOS 18.2+iPadOS 18.2+

``` source
case notAuthorized
```

## Discussion

The requested operation isn’t authorized; use requestAuthorization(for:) to request someone’s authorization to be able to send background messages from this app.

## See Also

### Error codes

case unknown

The error code the framework returns after an unknown error occurs.

case invalidAuthenticationRequest

The authentication request isn’t valid.

case notSupported

The framework doesn’t support the current device.

case sendFailed

The message failed to send.

