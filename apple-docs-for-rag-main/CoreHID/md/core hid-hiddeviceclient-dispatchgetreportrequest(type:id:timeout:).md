

- Core HID
- HIDDeviceClient
-  dispatchGetReportRequest(type:id:timeout:) 

Instance Method

# dispatchGetReportRequest(type:id:timeout:)

Send a get report request to the device over the transport.

macOS 15.0+

``` source
func dispatchGetReportRequest(
    type: HIDReportType,
    id: HIDReportID? = nil,
    timeout: Duration? = nil
) async throws -> Data
```

## Parameters 

`type`  

The HIDReportType of the requested report.

`id`  

The ID of the requested report, determined from the report descriptor. This is unnecessary if the descriptor has only one report.

`timeout`  

The maximum amount of time to wait for the device to receive the report before the call times out and fails. Not providing a duration causes the call to wait forever.

## Return Value

The data that the device returned. Reference the device’s descriptor to determine what data the device may respond with.

## Mentioned in 

Creating virtual devices

Communicating with human interface devices

## Discussion

Many HID devices respond to get report requests to retrieve information from the device. Exactly how a device responds to a get report request is dependent on the device specific implementation, but most devices conform to the reports that they declare in their report descriptor. This function throws if the device is seized by another client.

For more details, see Human Interface Devices (HID) Specifications and Tools.

Throws

HIDDeviceError if there is an issue with the request.

## See Also

### Interact with the device

func dispatchSetReportRequest(type: HIDReportType, id: HIDReportID?, data: Data, timeout: Duration?) async throws

Send a set report request to the device over the transport.

func seizeDevice() throws

Attempt to obtain the device so that this client is the only active client.

