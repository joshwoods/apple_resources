

- Core Bluetooth
- CBCentralManager
-  retrieveConnectedPeripherals(withServices:) 

Instance Method

# retrieveConnectedPeripherals(withServices:)

Returns a list of the peripherals connected to the system whose services match a given set of criteria.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func retrieveConnectedPeripherals(withServices serviceUUIDs: [CBUUID]) -> [CBPeripheral]
```

## Parameters 

`serviceUUIDs`  

A list of service UUIDs, represented by CBUUID objects.

## Return Value

A list of the peripherals that are currently connected to the system and that contain any of the services specified in the `serviceUUID` parameter.

## Discussion

The list of connected peripherals can include those that other apps have connected. You need to connect these peripherals locally using the connect(_:options:) method before using them.

## See Also

### Retrieving Lists of Peripherals

func retrievePeripherals(withIdentifiers: [UUID]) -> [CBPeripheral]

Returns a list of known peripherals by their identifiers.

