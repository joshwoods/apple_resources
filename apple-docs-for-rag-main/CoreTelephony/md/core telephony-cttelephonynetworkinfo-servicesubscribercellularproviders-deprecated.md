

- Core Telephony
- CTTelephonyNetworkInfo
-  serviceSubscriberCellularProviders Deprecated

Instance Property

# serviceSubscriberCellularProviders

A dictionary that contains carrier information about each service.

iOS 12.0–16.0DeprecatediPadOS 12.0–16.0DeprecatedMac Catalyst 13.1–16.0Deprecated

``` source
var serviceSubscriberCellularProviders: [String : CTCarrier]? { get }
```

Deprecated

Deprecated with no replacement

## Discussion

The keys for the serviceSubscriberCellularProviders dictionary are NSString objects, each of which represents a service. Each entry in the dictionary is a CTCarrier object, which contains information about the subscriber’s home cellular service provider.

Note

In this context, the “home” provider is the one with which the user has a cellular plan, as opposed to a roaming provider.

Although the actual value of a key isn’t important, you can also use it to get the current radio access technology associated with the service. To do so, pass the key to the serviceCurrentRadioAccessTechnology dictionary.

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

var serviceSubscriberCellularProvidersDidUpdateNotifier: ((String) -> Void)?

A block dispatched when there are updates to the user’s cellular provider information for any service.

Deprecated

static let CTRadioAccessTechnologyDidChange: NSNotification.Name

The name of the notification indicating that the radio access technology changed for one of the services.

Deprecated

