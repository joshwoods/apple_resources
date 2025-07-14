

- ImageCaptureCore
- ICScannerDeviceDelegate
-  scannerDevice(\_:didCompleteOverviewScanWithError:) 

Instance Method

# scannerDevice(\_:didCompleteOverviewScanWithError:)

Tells the client when the scanner completes an overview scan.

macOS 10.4+

``` source
optional func scannerDevice(
    _ scanner: ICScannerDevice,
    didCompleteOverviewScanWithError error: (any Error)?
)
```

## See Also

### Performing a Scan

func scannerDevice(ICScannerDevice, didCompleteScanWithError: (any Error)?)

Tells the client when the scanner completes a scan.

func scannerDevice(ICScannerDevice, didScanTo: ICScannerBandData)

Tells the client when the scanner receives the requested scan progress notification and a band of data is sent for each notification received.

func scannerDevice(ICScannerDevice, didScanTo: URL)

Tells the client when the scanner receives the requested scan.

