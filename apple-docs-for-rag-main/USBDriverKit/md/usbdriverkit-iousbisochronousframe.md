

- USBDriverKit
-  IOUSBIsochronousFrame 

Structure

# IOUSBIsochronousFrame

A structure representing a single frame in an isochronous transfer.

DriverKit 19.0+

``` source
struct IOUSBIsochronousFrame;
```

## Topics

### Getting the Frame Properties

status

The completion status for this individual frame.

requestCount

The number of bytes to transfer for this frame.

completeCount

The number of bytes actually transferred for this frame.

reserved

Reserved for future use.

timeStamp

The frame’s observed completion time.

## See Also

### Interacting with Isochronous Endpoints

IsochIO

Performs a synchronous or asynchronous request on an isochronous endpoint.

CompleteAsyncIsochIO

Handles the completion of an asynchronous request.

