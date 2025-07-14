

- USBDriverKit
- IOUSBHostPipe
-  IsochIO 

Instance Method

# IsochIO

Performs a synchronous or asynchronous request on an isochronous endpoint.

DriverKit 19.0+

``` source
kern_return_t IsochIO(IOMemoryDescriptor * dataBuffer, IOMemoryDescriptor * frameList, uint64_t firstFrameNumber, OSAction * completion);
```

## Parameters 

`dataBuffer`  

The buffer to store the data. When transferring data to the device, this buffer contains the data to send. When receiving data from the device, this buffer is empty initially.

`frameList`  

A valid memory descriptor containing the frame list, which is an array of IOUSBIsochronousFrame structures. For example, a frame list with 8 frames should be of size `(sizeof(IOUSBIsochronousFrame) * 8)`.

`firstFrameNumber`  

The starting frame number for the request. You can get the current frame number from the GetFrameNumber method of IOUSBHostDevice or IOUSBHostInterface. Specify `0` to begin the transfer on the next available frame (XHCI only).

`completion`  

An optional completion handler. To create a synchronous I/O request, specify `NULL`. To create an asynchronous request, provide an appropriate action method with your callback routine. This method copies your action object, so you can allocate that object on the stack if you prefer.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Use this method to issue isochronous requests. Allocate and initialize an array of IOUSBIsochronousFrame structures, which describe the frames to transfer. See IOUSBIsochronousFrame for information regarding structure initialization requirements and usage.

## See Also

### Interacting with Isochronous Endpoints

CompleteAsyncIsochIO

Handles the completion of an asynchronous request.

IOUSBIsochronousFrame

A structure representing a single frame in an isochronous transfer.

