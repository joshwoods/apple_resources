

- Core Telephony
- CTSubscriber
-  refreshCarrierToken() 

Instance Method

# refreshCarrierToken()

Attempts to refresh the carrier token.

iOS 6.0+iPadOS 6.0+

``` source
func refreshCarrierToken() -> Bool
```

## Return Value

`true` if the system performs a token refresh in response to this call; otherwise, `false`.

## Discussion

Call this method to update the carrierToken when the token exists but the server rejects it.

Note

Retrieve and attempt to use `carrierToken` first. Only call this method when you know the token is invalid.

Inspect the return value to determine whether this call results in an actual refresh. If the return value is `true`, the system attempts the refresh and calls the delegate method subscriberTokenRefreshed(_:). A return value of `false` indicates an invalid argument (such as bad carrier descriptors or service descriptor) or that the subscriber doesn’t support the authentication action.

## See Also

### Managing the carrier token

var carrierToken: Data?

A data object containing authorization information about the subscriber.

let CTSubscriberTokenRefreshed: String

The name of the notification indicating that the carrier token is available.

Deprecated

