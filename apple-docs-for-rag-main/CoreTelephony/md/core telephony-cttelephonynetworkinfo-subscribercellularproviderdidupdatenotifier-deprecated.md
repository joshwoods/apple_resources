

- Core Telephony
- CTTelephonyNetworkInfo
-  subscriberCellularProviderDidUpdateNotifier Deprecated

Instance Property

# subscriberCellularProviderDidUpdateNotifier

A block dispatched when the user’s cellular service provider information changes.

iOS 4.0–12.0DeprecatediPadOS 4.0–12.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var subscriberCellularProviderDidUpdateNotifier: ((CTCarrier) -> Void)? { get set }
```

Deprecated

Use serviceSubscriberCellularProvidersDidUpdateNotifier instead.

## Discussion

This block executes on the default priority global dispatch queue when the user’s cellular provider information changes. This occurs, for example, if a user swaps the device’s SIM card with one from another provider, while your app is running.

To handle changes in cellular service provider information, define a block in your app and assign it to this property. Implement the block to support being called from any context.

## See Also

### Deprecated

var currentRadioAccessTechnology: String?

The current radio access technology registered with the device.

Deprecated

var subscriberCellularProvider: CTCarrier?

Information about the user’s cellular service provider.

Deprecated

var serviceSubscriberCellularProviders: [String : CTCarrier]?

A dictionary that contains carrier information about each service.

Deprecated

var serviceSubscriberCellularProvidersDidUpdateNotifier: ((String) -> Void)?

A block dispatched when there are updates to the user’s cellular provider information for any service.

Deprecated

static let CTRadioAccessTechnologyDidChange: NSNotification.Name

The name of the notification indicating that the radio access technology changed for one of the services.

Deprecated

