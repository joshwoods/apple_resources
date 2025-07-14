

- Core Telephony
-  CTTelephonyNetworkInfoDelegate 

Protocol

# CTTelephonyNetworkInfoDelegate

The methods that the system invokes when data service changes occur.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
protocol CTTelephonyNetworkInfoDelegate : NSObjectProtocol
```

## Topics

### Responding to Data Service Changes

func dataServiceIdentifierDidChange(String)

Informs the delegate when the identifier changes for the service that’s currently providing data.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Getting Information About the Cellular Service Provider

var dataServiceIdentifier: String?

The identifier of the service that’s currently providing data.

var delegate: (any CTTelephonyNetworkInfoDelegate)?

An object that the system notifies when the data service identifier changes.

var serviceCurrentRadioAccessTechnology: [String : String]?

A dictionary containing the current radio access technology registered to each service.

Radio Access Technology Constants

Constants that describe the current radio access technology.

