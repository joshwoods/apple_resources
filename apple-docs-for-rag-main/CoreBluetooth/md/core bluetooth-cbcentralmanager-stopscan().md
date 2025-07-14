

- Core Bluetooth
- CBCentralManager
-  stopScan() 

Instance Method

# stopScan()

Asks the central manager to stop scanning for peripherals.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func stopScan()
```

## See Also

### Scanning or Stopping Scans of Peripherals

func scanForPeripherals(withServices: [CBUUID]?, options: [String : Any]?)

Scans for peripherals that are advertising services.

Peripheral Scanning Options

Keys used to pass options when scanning for peripherals.

var isScanning: Bool

A Boolean value that indicates whether the central is currently scanning.

