

- ImageCaptureCore
- ICScannerDevice
-  cancelScan() 

Instance Method

# cancelScan()

Cancels the current scan.

macOS 10.4+

``` source
func cancelScan()
```

## Discussion

Cancels the scan in progress by calling requestOverviewScan() or requestScan().

## See Also

### Performing a Scan

func requestOpenSession(withCredentials: String, password: String)

Opens a session on the protected device with the authorized username and passcode.

func requestOverviewScan()

Starts an overview scan on the selected functional unit.

func requestScan()

Starts a scan on the selected functional unit.

var documentName: String

The document’s name.

var documentUTI: String

The document’s uniform type identifier.

var downloadsDirectory: URL

The downloads directory.

var transferMode: ICScannerTransferMode

The transfer mode for the scanned document.

var maxMemoryBandSize: UInt32

The total maximum band size requested when performing a memory-based transfer.

