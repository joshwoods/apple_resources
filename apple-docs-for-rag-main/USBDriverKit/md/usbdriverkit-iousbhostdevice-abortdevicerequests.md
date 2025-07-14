

- USBDriverKit
- IOUSBHostDevice
-  AbortDeviceRequests 

Instance Method

# AbortDeviceRequests

Aborts device requests that you made previously from the current device client.

DriverKit 19.0+

``` source
kern_return_t AbortDeviceRequests(IOService * forClient, IOOptionBits options, IOReturn withError);
```

## Parameters 

`forClient`  

The client that issued the requests.

`options`  

Options to use when aborting requests. Specify `0` for this parameter.

`withError`  

The error value to report for each request. Specify `kIOReturnAborted` for this parameter.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Use this method to abort any requests you made previously with the AsyncDeviceRequest method. This method aborts only the requests that the current device object initiated.

## See Also

### Requesting Information from the Device

DeviceRequest

Sends a synchronous request to the device on the default control endpoint.

AsyncDeviceRequest

Enqueues a request on the default control endpoint of the device.

CompleteAsyncDeviceRequest

The type definition for an asynchronous device request completion routine.

