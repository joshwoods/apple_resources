

- USBDriverKit
- IOUSBHostPipe
-  CompleteAsyncIsochIO 

Instance Method

# CompleteAsyncIsochIO

Handles the completion of an asynchronous request.

DriverKit 19.0+

``` source
void CompleteAsyncIsochIO(OSAction * action, IOReturn status);
```

## Parameters 

`action`  

A pointer to the OSAction object of the request.

`status`  

The result of the operation.

## Discussion

Implement a custom version of this method and use the TYPE macro to let the system know that your method conforms to this prototype.

## See Also

### Interacting with Isochronous Endpoints

IsochIO

Performs a synchronous or asynchronous request on an isochronous endpoint.

IOUSBIsochronousFrame

A structure representing a single frame in an isochronous transfer.

