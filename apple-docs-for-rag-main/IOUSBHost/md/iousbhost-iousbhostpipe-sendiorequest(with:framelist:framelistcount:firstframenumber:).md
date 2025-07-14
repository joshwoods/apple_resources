

- IOUSBHost
- IOUSBHostPipe
-  sendIORequest(with:frameList:frameListCount:firstFrameNumber:) 

Instance Method

# sendIORequest(with:frameList:frameListCount:firstFrameNumber:)

Sends a request on an isochronous endpoint.

Mac Catalyst 14.0+macOS 10.15–11.0Deprecated

``` source
func sendIORequest(
    with data: NSMutableData,
    frameList: UnsafeMutablePointer,
    frameListCount: Int,
    firstFrameNumber: UInt64
) throws
```

## Parameters 

`data`  

An NSMutableData object defining the memory to use for the transfer.

`frameList`  

A pointer to the first element in an IOUSBHostIsochronousFrame array. The array must contain at least `frameListCount` elements.

`frameListCount`  

The number of elements in `frameList`.

`firstFrameNumber`  

The frame number the request begins on. Query the current frame number with frameNumberWithTime:. If `0`, the transfer starts on the next available frame (XHCI only).

## Discussion

This method issues synchronous isochronous requests. The caller allocates and initializes an array of IOUSBHostIsochronousFrame structures to describe the transferred frames.

## See Also

### Sending Isochronous I/O

typealias IOUSBHostIsochronousCompletionHandler

A completion handler for asynchronous isochronous transfers.

typealias IOUSBHostTime

The absolute time.

struct IOUSBHostIsochronousFrame

A structure that represents a single frame in an isochronous transfer.

func enqueueIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64, completionHandler: IOUSBHostIsochronousCompletionHandler?) throws

Enqueues a request on an isochronous endpoint.

