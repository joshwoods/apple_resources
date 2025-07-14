

- Messages
- MSCriticalMessagingError
-  MSCriticalMessagingError.sendFailed 

Case

# MSCriticalMessagingError.sendFailed

The message failed to send.

iOS 18.2+iPadOS 18.2+

``` source
case sendFailed
```

## Mentioned in 

Sending SMS messages from an app

## Discussion

The framework isn’t able to send the message for one of the following reasons:

- An unreachable or incorrectly formatted phone number

- An unavailable cellular network

- The device’s SIM is in a disabled state

Note

The phone number needs to conform to the ITU E.164 telephone numbering plan standard, without any additional non-numeric characters such as dashes, periods, parentheses, or a plus character (+) that introduces a country code.

## See Also

### Error codes

case unknown

The error code the framework returns after an unknown error occurs.

case invalidAuthenticationRequest

The authentication request isn’t valid.

case notSupported

The framework doesn’t support the current device.

case notAuthorized

The operation isn’t authorized.

