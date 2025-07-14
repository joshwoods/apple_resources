

- Core HID
- HIDDeviceClient
-  seizeDevice() 

Instance Method

# seizeDevice()

Attempt to obtain the device so that this client is the only active client.

macOS 15.0+

``` source
func seizeDevice() throws
```

## Discussion

If successful, this client is the only one that receives notifications using monitorNotifications(reportIDsToMonitor:elementsToMonitor:), and the only one that can use certain functions to interact with the device. The device won’t be freed until the client that holds it is deinitialized. There must not be any outstanding calls when attempting to seize a device.

Throws

HIDDeviceError if the attempt to seize the device is unsuccessful. Notably, HIDDeviceError.busy is thrown if there are outstanding calls to monitorNotifications(reportIDsToMonitor:elementsToMonitor:), dispatchSetReportRequest(type:id:data:timeout:), dispatchGetReportRequest(type:id:timeout:), or updateElements(_:timeout:); and HIDDeviceError.exclusiveAccess is thrown if the device is currently seized by another client.

## See Also

### Interact with the device

func dispatchGetReportRequest(type: HIDReportType, id: HIDReportID?, timeout: Duration?) async throws -> Data

Send a get report request to the device over the transport.

func dispatchSetReportRequest(type: HIDReportType, id: HIDReportID?, data: Data, timeout: Duration?) async throws

Send a set report request to the device over the transport.

