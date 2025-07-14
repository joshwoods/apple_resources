

- ImageCaptureCore
-  ICScannerDeviceDelegate 

Protocol

# ICScannerDeviceDelegate

Methods for determining availability, selecting a functional unit, and performing scans on connected scanners.

macOS 10.4+

``` source
protocol ICScannerDeviceDelegate : ICDeviceDelegate
```

## Topics

### Determining Scanner Availability

func scannerDeviceDidBecomeAvailable(ICScannerDevice)

Tells the client when another client closes the current open session on the scanner.

### Selecting a Functional Unit

func scannerDevice(ICScannerDevice, didSelect: ICScannerFunctionalUnit, error: (any Error)?)

Tells the client when a functional unit is selected on the scanner.

### Performing a Scan

func scannerDevice(ICScannerDevice, didCompleteOverviewScanWithError: (any Error)?)

Tells the client when the scanner completes an overview scan.

func scannerDevice(ICScannerDevice, didCompleteScanWithError: (any Error)?)

Tells the client when the scanner completes a scan.

func scannerDevice(ICScannerDevice, didScanTo: ICScannerBandData)

Tells the client when the scanner receives the requested scan progress notification and a band of data is sent for each notification received.

func scannerDevice(ICScannerDevice, didScanTo: URL)

Tells the client when the scanner receives the requested scan.

## Relationships

### Inherits From

- ICDeviceDelegate
- NSObjectProtocol

## See Also

### Scanners

class ICScannerDevice

An object that represents a scanner.

Scanner Configuration

Examine a scanner’s functional units and features.

