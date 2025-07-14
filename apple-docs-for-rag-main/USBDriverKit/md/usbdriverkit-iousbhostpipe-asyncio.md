

- USBDriverKit
- IOUSBHostPipe
-  AsyncIO 

Instance Method

# AsyncIO

Enqueues an asynchronous request on a bulk or interrupt endpoint.

DriverKit 19.0+

``` source
kern_return_t AsyncIO(IOMemoryDescriptor * dataBuffer, uint32_t dataBufferLength, OSAction * completion, uint32_t completionTimeoutMs);
```

## Parameters 

`dataBuffer`  

The data buffer to use for the request. When transferring data to the device, this buffer contains the data to send. When receiving data from the device, this buffer is empty initially.

`dataBufferLength`  

The length of the data buffer.

`completion`  

An action object containing the callback method to execute when the transfer finishes.

`completionTimeoutMs`  

The timeout value in milliseconds. Specify `0` if you don’t want the request to time out. You must specify `0` when transferring data on an interrupt endpoint.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method performs an appropriate USB I/O request on the device and notifies your completion handler asynchronously when that transfer completes.

## See Also

### Interacting with Bulk and Interrupt Endpoints

IO

Performs a synchronous request on a bulk or interrupt endpoint.

CompleteAsyncIO

Handles the completion of an asynchronous I/O request.

