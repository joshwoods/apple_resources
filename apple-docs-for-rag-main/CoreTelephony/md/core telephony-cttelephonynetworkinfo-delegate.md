

- Core Telephony
- CTTelephonyNetworkInfo
-  delegate 

Instance Property

# delegate

An object that the system notifies when the data service identifier changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
weak var delegate: (any CTTelephonyNetworkInfoDelegate)? { get set }
```

## See Also

### Getting Information About the Cellular Service Provider

var dataServiceIdentifier: String?

The identifier of the service that’s currently providing data.

protocol CTTelephonyNetworkInfoDelegate

The methods that the system invokes when data service changes occur.

var serviceCurrentRadioAccessTechnology: [String : String]?

A dictionary containing the current radio access technology registered to each service.

Radio Access Technology Constants

Constants that describe the current radio access technology.

