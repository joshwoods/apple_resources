

- ImageCaptureCore
- ICScannerDevice
-  documentName 

Instance Property

# documentName

The document’s name.

macOS 10.4+

``` source
var documentName: String { get set }
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

var documentUTI: String

The document’s uniform type identifier.

var downloadsDirectory: URL

The downloads directory.

var transferMode: ICScannerTransferMode

The transfer mode for the scanned document.

var maxMemoryBandSize: UInt32

The total maximum band size requested when performing a memory-based transfer.

