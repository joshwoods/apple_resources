

- Core HID
- HIDVirtualDevice
-  dispatchInputReport(data:timestamp:) 

Instance Method

# dispatchInputReport(data:timestamp:)

Dispatch an input report to the system.

macOS 15.0+

``` source
func dispatchInputReport(
    data: Data,
    timestamp: SuspendingClock.Instant
) async throws
```

## Parameters 

`data`  

The bytes to send as a part of the input report. Determining the correct values can be aided by referencing the device’s report descriptor. If there are multiple reports, the first byte should be the report ID.

`timestamp`  

The time that the report originated.

## Discussion

This dispatches an input report to the system, as if a person is interacting with a physical control. For example, if the virtual device represents a keyboard, a keyboard report can be dispatched here to simulate a person pressing a key on the keyboard. The system receives the report and any HIDDeviceClient devices monitoring for such activity. activate(delegate:) must run successfully before this function runs.

Throws

HIDDeviceError if there is an issue with the request.

