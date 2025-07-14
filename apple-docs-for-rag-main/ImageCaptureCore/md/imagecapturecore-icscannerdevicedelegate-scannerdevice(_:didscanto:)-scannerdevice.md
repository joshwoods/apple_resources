

- ImageCaptureCore
- ICScannerDeviceDelegate
-  scannerDevice(\_:didScanTo:) 

Instance Method

# scannerDevice(\_:didScanTo:)

Tells the client when the scanner receives the requested scan progress notification and a band of data is sent for each notification received.

macOS 10.7+

``` source
optional func scannerDevice(
    _ scanner: ICScannerDevice,
    didScanTo data: ICScannerBandData
)
```

## Discussion

In memory transfer mode, this method sends a band of the size selected by the client using the maxMemoryBandSize property.

## See Also

### Performing a Scan

func scannerDevice(ICScannerDevice, didCompleteOverviewScanWithError: (any Error)?)

Tells the client when the scanner completes an overview scan.

func scannerDevice(ICScannerDevice, didCompleteScanWithError: (any Error)?)

Tells the client when the scanner completes a scan.

func scannerDevice(ICScannerDevice, didScanTo: URL)

Tells the client when the scanner receives the requested scan.

