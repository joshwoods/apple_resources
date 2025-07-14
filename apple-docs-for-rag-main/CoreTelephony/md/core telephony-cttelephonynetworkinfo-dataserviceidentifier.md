

- Core Telephony
- CTTelephonyNetworkInfo
-  dataServiceIdentifier 

Instance Property

# dataServiceIdentifier

The identifier of the service that’s currently providing data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var dataServiceIdentifier: String? { get }
```

## See Also

### Getting Information About the Cellular Service Provider

var delegate: (any CTTelephonyNetworkInfoDelegate)?

An object that the system notifies when the data service identifier changes.

protocol CTTelephonyNetworkInfoDelegate

The methods that the system invokes when data service changes occur.

var serviceCurrentRadioAccessTechnology: [String : String]?

A dictionary containing the current radio access technology registered to each service.

Radio Access Technology Constants

Constants that describe the current radio access technology.

