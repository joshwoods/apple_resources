

- IOUSBHost
-  IOUSBHostIsochronousCompletionHandler 

Type Alias

# IOUSBHostIsochronousCompletionHandler

A completion handler for asynchronous isochronous transfers.

Mac Catalyst 14.0+macOS 10.15+

``` source
typealias IOUSBHostIsochronousCompletionHandler = (IOReturn, UnsafeMutablePointer) -> Void
```

## Parameters 

`status`  

The result code for isochronous transfer.

`frameList`  

The frame list of IOUSBHostIsochronousFrame that enqueueIORequest(with:frameList:frameListCount:firstFrameNumber:completionHandler:) passes.

## See Also

### Sending Isochronous I/O

typealias IOUSBHostTime

The absolute time.

struct IOUSBHostIsochronousFrame

A structure that represents a single frame in an isochronous transfer.

func enqueueIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64, completionHandler: IOUSBHostIsochronousCompletionHandler?) throws

Enqueues a request on an isochronous endpoint.

func sendIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64) throws

Sends a request on an isochronous endpoint.

