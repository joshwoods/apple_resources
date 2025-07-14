

- Core Telephony
- CTTelephonyNetworkInfo
-  serviceSubscriberCellularProvidersDidUpdateNotifier Deprecated

Instance Property

# serviceSubscriberCellularProvidersDidUpdateNotifier

A block dispatched when there are updates to the user’s cellular provider information for any service.

iOS 12.0–16.0DeprecatediPadOS 12.0–16.0DeprecatedMac Catalyst 13.1–16.0Deprecated

``` source
var serviceSubscriberCellularProvidersDidUpdateNotifier: ((String) -> Void)? { get set }
```

Deprecated

Deprecated with no replacement

## Discussion

The block object executes on the default priority global dispatch queue when the user’s cellular provider information changes. This occurs, for example, if a user swaps the device’s SIM card with one from another provider, while your app is running.

To handle changes in cellular service provider information, define a block in your app and assign it to this property. Implement the block to support being called from any context. To get the new information, use the NSString (which contains the identifier of the service whose information has changed) as the key into serviceSubscriberCellularProviders.

## See Also

### Deprecated

var currentRadioAccessTechnology: String?

The current radio access technology registered with the device.

Deprecated

var subscriberCellularProvider: CTCarrier?

Information about the user’s cellular service provider.

Deprecated

var subscriberCellularProviderDidUpdateNotifier: ((CTCarrier) -> Void)?

A block dispatched when the user’s cellular service provider information changes.

Deprecated

var serviceSubscriberCellularProviders: [String : CTCarrier]?

A dictionary that contains carrier information about each service.

Deprecated

static let CTRadioAccessTechnologyDidChange: NSNotification.Name

The name of the notification indicating that the radio access technology changed for one of the services.

Deprecated

