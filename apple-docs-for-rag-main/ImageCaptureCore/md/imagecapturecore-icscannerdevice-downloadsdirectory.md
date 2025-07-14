

- ImageCaptureCore
- ICScannerDevice
-  downloadsDirectory 

Instance Property

# downloadsDirectory

The downloads directory.

macOS 10.4+

``` source
var downloadsDirectory: URL { get set }
```

## See Also

### Performing a Scan

func requestOpenSession(withCredentials: String, password: String)

Opens a session on the protected device with the authorized username and passcode.

func requestOverviewScan()

Starts an overview scan on the selected functional unit.

func requestScan()

Starts a scan on the selected functional unit.

func cancelScan()

Cancels the current scan.

var documentName: String

The document’s name.

var documentUTI: String

The document’s uniform type identifier.

var transferMode: ICScannerTransferMode

The transfer mode for the scanned document.

var maxMemoryBandSize: UInt32

The total maximum band size requested when performing a memory-based transfer.

