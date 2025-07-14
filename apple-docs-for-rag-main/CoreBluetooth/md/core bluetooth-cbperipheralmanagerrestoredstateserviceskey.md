

- Core Bluetooth
-  CBPeripheralManagerRestoredStateServicesKey 

Global Variable

# CBPeripheralManagerRestoredStateServicesKey

An array of restored peripheral services.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBPeripheralManagerRestoredStateServicesKey: String
```

## Discussion

The value associated with this key is an NSArray of CBMutableService objects. It contains all of the services that previously published to the local peripheral’s database when the system quit the app.

Restoration includes all information about a service, including any included services, characteristics, characteristic descriptors, and subscribed centrals.

## See Also

### State Restoration Dictionary Keys

let CBPeripheralManagerRestoredStateAdvertisementDataKey: String

A dictionary of restored advertising data.

