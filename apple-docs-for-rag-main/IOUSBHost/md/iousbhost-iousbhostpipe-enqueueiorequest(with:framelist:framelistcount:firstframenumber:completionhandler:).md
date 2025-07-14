

- IOUSBHost
- IOUSBHostPipe
-  enqueueIORequest(with:frameList:frameListCount:firstFrameNumber:completionHandler:) 

Instance Method

# enqueueIORequest(with:frameList:frameListCount:firstFrameNumber:completionHandler:)

Enqueues a request on an isochronous endpoint.

Mac Catalyst 14.0+macOS 10.15–11.0Deprecated

``` source
func enqueueIORequest(
    with data: NSMutableData,
    frameList: UnsafeMutablePointer,
    frameListCount: Int,
    firstFrameNumber: UInt64,
    completionHandler: IOUSBHostIsochronousCompletionHandler? = nil
) throws
```

``` source
func enqueueIORequest(
    with data: NSMutableData,
    frameList: UnsafeMutablePointer,
    frameListCount: Int,
    firstFrameNumber: UInt64
) async throws -> (IOReturn, UnsafeMutablePointer)
```

## Parameters 

`data`  

An NSMutableData object defining the memory to use for the transfer.

`frameList`  

A pointer to the first element in an IOUSBHostIsochronousFrame array. The array must contain at least `frameListCount` elements.

`frameListCount`  

The number of elements in `frameList`.

`firstFrameNumber`  

The frame number the request should begin on. Query the current frame number with frameNumberWithTime:. If `0`, the transfer starts on the next available frame (XHCI only).

`completionHandler`  

An IOUSBHostIsochronousCompletionHandler that runs when the request completes, or times out if the call returns successfully. The `completionHandler` doesn’t run if the method returns with an error.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func enqueueIORequest(with data: NSMutableData, frameList: UnsafeMutablePointer, frameListCount: Int, firstFrameNumber: UInt64) async throws -> (IOReturn, UnsafeMutablePointer)
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method issues asynchronous isochronous requests. The caller allocates and initializes an array of IOUSBHostIsochronousFrame structures to describe the transferred frames.

## See Also

### Sending Isochronous I/O

typealias IOUSBHostIsochronousCompletionHandler

A completion handler for asynchronous isochronous transfers.

typealias IOUSBHostTime

The absolute time.

struct IOUSBHostIsochronousFrame

A structure that represents a single frame in an isochronous transfer.

func sendIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64) throws

Sends a request on an isochronous endpoint.

