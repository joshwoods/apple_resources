

- USBDriverKit
- IOUSBHostDevice
-  CompleteAsyncDeviceRequest 

Instance Method

# CompleteAsyncDeviceRequest

The type definition for an asynchronous device request completion routine.

DriverKit 19.0+

``` source
void CompleteAsyncDeviceRequest(OSAction * action, IOReturn status, uint32_t bytesTransferred);
```

## Parameters 

`action`  

A pointer to the `OSAction` object of the async request.

`status`  

The result of the operation.

`bytesTransferred`  

The byte count of the completed data phase.

## Discussion

Implement a custom version of this method and use the TYPE macro to let the system know that your method conforms to this prototype.

## See Also

### Requesting Information from the Device

DeviceRequest

Sends a synchronous request to the device on the default control endpoint.

AsyncDeviceRequest

Enqueues a request on the default control endpoint of the device.

AbortDeviceRequests

Aborts device requests that you made previously from the current device client.

