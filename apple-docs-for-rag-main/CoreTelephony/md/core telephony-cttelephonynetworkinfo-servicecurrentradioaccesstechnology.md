

- Core Telephony
- CTTelephonyNetworkInfo
-  serviceCurrentRadioAccessTechnology 

Instance Property

# serviceCurrentRadioAccessTechnology

A dictionary containing the current radio access technology registered to each service.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var serviceCurrentRadioAccessTechnology: [String : String]? { get }
```

## Discussion

The keys for the serviceCurrentRadioAccessTechnology dictionary are NSString objects, each of which represents a service. The entry associated with a key is `nil` if the service is not registered on any network.

Although the actual value of a key isn’t important, you can also use it to get the carrier information associated with the service. To do so, pass the key to the serviceSubscriberCellularProviders dictionary.

## See Also

### Getting Information About the Cellular Service Provider

var dataServiceIdentifier: String?

The identifier of the service that’s currently providing data.

var delegate: (any CTTelephonyNetworkInfoDelegate)?

An object that the system notifies when the data service identifier changes.

protocol CTTelephonyNetworkInfoDelegate

The methods that the system invokes when data service changes occur.

Radio Access Technology Constants

Constants that describe the current radio access technology.

