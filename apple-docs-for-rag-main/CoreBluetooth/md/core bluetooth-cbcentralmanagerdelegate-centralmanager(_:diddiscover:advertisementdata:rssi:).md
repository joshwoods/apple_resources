

- Core Bluetooth
- CBCentralManagerDelegate
-  centralManager(\_:didDiscover:advertisementData:rssi:) 

Instance Method

# centralManager(\_:didDiscover:advertisementData:rssi:)

Tells the delegate the central manager discovered a peripheral while scanning for devices.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func centralManager(
    _ central: CBCentralManager,
    didDiscover peripheral: CBPeripheral,
    advertisementData: [String : Any],
    rssi RSSI: NSNumber
)
```

## Parameters 

`central`  

The central manager that provides the update.

`peripheral`  

The discovered peripheral.

`advertisementData`  

A dictionary containing any advertisement data.

`RSSI`  

The current received signal strength indicator (RSSI) of the peripheral, in decibels.

## Discussion

You can access the advertisement data with the keys listed in Advertisement Data Retrieval Keys. You must retain a local copy of the peripheral if you want to perform commands on it. Use the RSSI data to determine the proximity of a discoverable peripheral device, and whether you want to connect to it automatically.

## See Also

### Discovering and Retrieving Peripherals

Advertisement Data Retrieval Keys

Keys used to specify items in a dictionary of peripheral advertisement data.

