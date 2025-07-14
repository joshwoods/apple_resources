

- Core Telephony
-  CTSubscriberTokenRefreshed Deprecated

Global Variable

# CTSubscriberTokenRefreshed

The name of the notification indicating that the carrier token is available.

iOS 7.0–12.1DeprecatediPadOS 7.0–12.1DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
let CTSubscriberTokenRefreshed: String
```

Deprecated

Use the CTSubscriberDelegate method subscriberTokenRefreshed(_:) instead.

## Discussion

The notification’s object property is the CTSubscriber instance whose subscriber token refreshed.

## See Also

### Managing the carrier token

var carrierToken: Data?

A data object containing authorization information about the subscriber.

func refreshCarrierToken() -> Bool

Attempts to refresh the carrier token.

