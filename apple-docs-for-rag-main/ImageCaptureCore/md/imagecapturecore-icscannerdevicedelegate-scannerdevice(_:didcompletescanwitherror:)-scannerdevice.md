

- ImageCaptureCore
- ICScannerDeviceDelegate
-  scannerDevice(\_:didCompleteScanWithError:) 

Instance Method

# scannerDevice(\_:didCompleteScanWithError:)

Tells the client when the scanner completes a scan.

macOS 10.4+

``` source
optional func scannerDevice(
    _ scanner: ICScannerDevice,
    didCompleteScanWithError error: (any Error)?
)
```

## See Also

### Performing a Scan

func scannerDevice(ICScannerDevice, didCompleteOverviewScanWithError: (any Error)?)

Tells the client when the scanner completes an overview scan.

func scannerDevice(ICScannerDevice, didScanTo: ICScannerBandData)

Tells the client when the scanner receives the requested scan progress notification and a band of data is sent for each notification received.

func scannerDevice(ICScannerDevice, didScanTo: URL)

Tells the client when the scanner receives the requested scan.

