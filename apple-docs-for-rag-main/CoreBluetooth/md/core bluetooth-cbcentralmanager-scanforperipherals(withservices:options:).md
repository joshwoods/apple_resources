

- Core Bluetooth
- CBCentralManager
-  scanForPeripherals(withServices:options:) 

Instance Method

# scanForPeripherals(withServices:options:)

Scans for peripherals that are advertising services.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func scanForPeripherals(
    withServices serviceUUIDs: [CBUUID]?,
    options: [String : Any]? = nil
)
```

## Parameters 

`serviceUUIDs`  

An array of CBUUID objects that the app is interested in. Each CBUUID object represents the UUID of a service that a peripheral advertises.

`options`  

A dictionary of options for customizing the scan. For available options, see Peripheral Scanning Options.

## Discussion

You can provide an array of CBUUID objects — representing service UUIDs — in the `serviceUUIDs` parameter. When you do, the central manager returns only peripherals that advertise the services you specify. If the `serviceUUIDs` parameter is `nil`, this method returns all discovered peripherals, regardless of their supported services.

Note

The recommended practice is to populate the `serviceUUIDs` parameter rather than leaving it `nil`.

If the central manager is actively scanning with one set of parameters and it receives another set to scan, the new parameters override the previous set. When the central manager discovers a peripheral, it calls the centralManager(_:didDiscover:advertisementData:rssi:) method of its delegate object.

Your app can scan for Bluetooth devices in the background by specifying the `bluetooth-central` background mode. To do this, your app must explicitly scan for one or more services by specifying them in the `serviceUUIDs` parameter. The CBCentralManager scan option has no effect while scanning in the background.

## See Also

### Scanning or Stopping Scans of Peripherals

Peripheral Scanning Options

Keys used to pass options when scanning for peripherals.

func stopScan()

Asks the central manager to stop scanning for peripherals.

var isScanning: Bool

A Boolean value that indicates whether the central is currently scanning.

