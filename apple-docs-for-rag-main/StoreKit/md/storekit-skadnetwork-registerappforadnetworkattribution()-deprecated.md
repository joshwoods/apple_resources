

- StoreKit
- SKAdNetwork
-  registerAppForAdNetworkAttribution() Deprecated

Type Method

# registerAppForAdNetworkAttribution()

Verifies the first launch of an app installed as a result of an ad.

iOS 11.3–15.4DeprecatediPadOS 11.3–15.4DeprecatedMac Catalyst 13.1–15.4Deprecated

``` source
class func registerAppForAdNetworkAttribution()
```

Deprecated

Use updatePostbackConversionValue(_:coarseValue:lockWindow:completionHandler:) instead.

## Discussion

Apps that an ad network campaign advertise call this method or updateConversionValue(_:) when the app first launches. Both methods generate an install notification, which is the cryptographically signed data that validates that a user installed and launched this app as a result of an ad.

In iOS 15.4 and earlier, the first call to registerAppForAdNetworkAttribution() generates the notification if the device has attribution data for that app, and starts a 24-hour timer. Subsequent calls to this method have no effect, unless the ad already has a conversion value set, in which case calling registerAppForAdNetworkAttribution() resets the conversion value to `0`. You may, however, call updateConversionValue(_:) to provide an updated conversion value and restart the timer.

The device sends one or more install notifications to ad network postback URLs within 0-24 hours after the timer expires. For more information about attribution-winning and non-winning postbacks, see Receiving ad attributions and postbacks.

Ad networks must verify the postback after receiving it. For more information, see Verifying an install-validation postback.

## See Also

### Deprecated

class func updateConversionValue(Int)

Updates the conversion value and verifies the first launch of an app installed as a result of an ad.

Deprecated

