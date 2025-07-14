

- Core Bluetooth
- CBCentralManager
-  retrievePeripherals(withIdentifiers:) 

Instance Method

# retrievePeripherals(withIdentifiers:)

Returns a list of known peripherals by their identifiers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func retrievePeripherals(withIdentifiers identifiers: [UUID]) -> [CBPeripheral]
```

## Parameters 

`identifiers`  

A list of peripheral identifiers (represented by NSUUID objects) from which CBPeripheral objects can be retrieved.

## Return Value

A list of peripherals that the central manager is able to match to the provided identifiers.

## See Also

### Retrieving Lists of Peripherals

func retrieveConnectedPeripherals(withServices: [CBUUID]) -> [CBPeripheral]

Returns a list of the peripherals connected to the system whose services match a given set of criteria.

