

- ImageCaptureCore
- ICScannerDevice
-  documentUTI 

Instance Property

# documentUTI

The document’s uniform type identifier.

macOS 10.4+

``` source
var documentUTI: String { get set }
```

## Discussion

Supported uniform type identifiers are `kUTTypeJPEG`, `kUTTypeJPEG2000`, `kUTTypeTIFF`, and `kUTTypePNG`.

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

var downloadsDirectory: URL

The downloads directory.

var transferMode: ICScannerTransferMode

The transfer mode for the scanned document.

var maxMemoryBandSize: UInt32

The total maximum band size requested when performing a memory-based transfer.

