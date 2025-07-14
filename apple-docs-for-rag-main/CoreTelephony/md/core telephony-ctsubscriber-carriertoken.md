

- Core Telephony
- CTSubscriber
-  carrierToken 

Instance Property

# carrierToken

A data object containing authorization information about the subscriber.

iOS 7.0+iPadOS 7.0+

``` source
var carrierToken: Data? { get }
```

## Discussion

May contain `nil` if no token is available.

The carrier API obtains this token from a carrier-provided server. The token authenticates your app to a server provided by the carrier, to prove that your app is running on a device owned by the subscriber.

## See Also

### Managing the carrier token

func refreshCarrierToken() -> Bool

Attempts to refresh the carrier token.

let CTSubscriberTokenRefreshed: String

The name of the notification indicating that the carrier token is available.

Deprecated

