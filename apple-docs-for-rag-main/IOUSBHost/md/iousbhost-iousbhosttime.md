

- IOUSBHost
-  IOUSBHostTime 

Type Alias

# IOUSBHostTime

The absolute time.

Mac Catalyst 14.0+macOS 10.15+

``` source
typealias IOUSBHostTime = UInt64
```

## See Also

### Sending Isochronous I/O

typealias IOUSBHostIsochronousCompletionHandler

A completion handler for asynchronous isochronous transfers.

struct IOUSBHostIsochronousFrame

A structure that represents a single frame in an isochronous transfer.

func enqueueIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64, completionHandler: IOUSBHostIsochronousCompletionHandler?) throws

Enqueues a request on an isochronous endpoint.

func sendIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64) throws

Sends a request on an isochronous endpoint.

