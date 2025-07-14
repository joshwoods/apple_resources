

- ImageCaptureCore
- ICScannerDevice
-  requestOpenSession(withCredentials:password:) 

Instance Method

# requestOpenSession(withCredentials:password:)

Opens a session on the protected device with the authorized username and passcode.

macOS 10.4+

``` source
func requestOpenSession(
    withCredentials username: String,
    password: String
)
```

## Discussion

If the device reports a failure of credentials, you can provide them here for the launch. A client must open a session on a device in order to use the device.

Before calling this method, set the receiver’s delegate; otherwise, the request is ignored.

Once the request to open the session has completed, device(_:didOpenSessionWithError:) is called on the delegate.

No more messages are sent to the delegate if this request fails.

## See Also

### Performing a Scan

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

var downloadsDirectory: URL

The downloads directory.

var transferMode: ICScannerTransferMode

The transfer mode for the scanned document.

var maxMemoryBandSize: UInt32

The total maximum band size requested when performing a memory-based transfer.

