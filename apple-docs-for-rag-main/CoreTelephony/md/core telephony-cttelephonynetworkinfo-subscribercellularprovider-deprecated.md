

- Core Telephony
- CTTelephonyNetworkInfo
-  subscriberCellularProvider Deprecated

Instance Property

# subscriberCellularProvider

Information about the user’s cellular service provider.

iOS 4.0–12.0DeprecatediPadOS 4.0–12.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var subscriberCellularProvider: CTCarrier? { get }
```

Deprecated

Use serviceSubscriberCellularProviders instead.

## Discussion

A CTCarrier object that contains information about the user’s home cellular service provider. The home provider is the provider with whom the user has an account. This information is available immediately after you allocate and initialize the CTTelephonyNetworkInfo object.

## See Also

### Deprecated

var currentRadioAccessTechnology: String?

The current radio access technology registered with the device.

Deprecated

var subscriberCellularProviderDidUpdateNotifier: ((CTCarrier) -> Void)?

A block dispatched when the user’s cellular service provider information changes.

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

