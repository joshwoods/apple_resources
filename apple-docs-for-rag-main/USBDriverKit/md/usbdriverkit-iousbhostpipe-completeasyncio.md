

- USBDriverKit
- IOUSBHostPipe
-  CompleteAsyncIO 

Instance Method

# CompleteAsyncIO

Handles the completion of an asynchronous I/O request.

DriverKit 19.0+

``` source
void CompleteAsyncIO(OSAction * action, IOReturn status, uint32_t actualByteCount, uint64_t completionTimestamp);
```

## Parameters 

`action`  

A pointer to the OSAction object of the request.

`status`  

The result of the operation.

`actualByteCount`  

The number of bytes that the operation actually transferred.

`completionTimestamp`  

The absolute time that the transfer completed.

## Discussion

Implement a custom version of this method and use the TYPE macro to let the system know that your method conforms to this prototype.

## See Also

### Interacting with Bulk and Interrupt Endpoints

IO

Performs a synchronous request on a bulk or interrupt endpoint.

AsyncIO

Enqueues an asynchronous request on a bulk or interrupt endpoint.

