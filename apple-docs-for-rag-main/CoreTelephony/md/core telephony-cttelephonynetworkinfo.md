

- Core Telephony
-  CTTelephonyNetworkInfo 

Class

# CTTelephonyNetworkInfo

An object that provides notifications of changes to the user’s cellular service provider.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
class CTTelephonyNetworkInfo
```

## Overview

Your app should be able to handle changes to the user’s cellular service provider. For example, the user could swap the device’s SIM card with one from another provider while your app is running.

This class also gives you access to the CTCarrier object, which contains information about the user’s home cellular service provider.

## Topics

### Getting Information About the Cellular Service Provider

var dataServiceIdentifier: String?

The identifier of the service that’s currently providing data.

var delegate: (any CTTelephonyNetworkInfoDelegate)?

An object that the system notifies when the data service identifier changes.

protocol CTTelephonyNetworkInfoDelegate

The methods that the system invokes when data service changes occur.

var serviceCurrentRadioAccessTechnology: [String : String]?

A dictionary containing the current radio access technology registered to each service.

Radio Access Technology Constants

Constants that describe the current radio access technology.

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

var serviceSubscriberCellularProvidersDidUpdateNotifier: ((String) -> Void)?

A block dispatched when there are updates to the user’s cellular provider information for any service.

Deprecated

static let CTRadioAccessTechnologyDidChange: NSNotification.Name

The name of the notification indicating that the radio access technology changed for one of the services.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Service Information

class CTCarrier

Information about the user’s cellular service provider, such as its unique identifier and whether it allows VoIP calls on its network.

Deprecated

