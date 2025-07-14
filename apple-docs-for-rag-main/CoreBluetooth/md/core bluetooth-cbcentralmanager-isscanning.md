

- Core Bluetooth
- CBCentralManager
-  isScanning 

Instance Property

# isScanning

A Boolean value that indicates whether the central is currently scanning.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.13+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isScanning: Bool { get }
```

## See Also

### Scanning or Stopping Scans of Peripherals

func scanForPeripherals(withServices: [CBUUID]?, options: [String : Any]?)

Scans for peripherals that are advertising services.

Peripheral Scanning Options

Keys used to pass options when scanning for peripherals.

func stopScan()

Asks the central manager to stop scanning for peripherals.

