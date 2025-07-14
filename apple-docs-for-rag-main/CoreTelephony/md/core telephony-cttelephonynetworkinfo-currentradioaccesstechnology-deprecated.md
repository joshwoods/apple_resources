

- Core Telephony
- CTTelephonyNetworkInfo
-  currentRadioAccessTechnology Deprecated

Instance Property

# currentRadioAccessTechnology

The current radio access technology registered with the device.

iOS 7.0–12.0DeprecatediPadOS 7.0–12.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var currentRadioAccessTechnology: String? { get }
```

Deprecated

Use serviceCurrentRadioAccessTechnology instead.

## Discussion

If the device isn’t registered on any network, this property is `nil`.

## See Also

### Deprecated

var subscriberCellularProvider: CTCarrier?

Information about the user’s cellular service provider.

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

