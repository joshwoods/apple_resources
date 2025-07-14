

- HIDDriverKit
- IOUserHIDEventService
-  dispatchDigitizerStylusEvent 

Instance Method

# dispatchDigitizerStylusEvent

Dispatches a digitizer stylus event to the system.

DriverKit 19.0+macOS

``` source
kern_return_t dispatchDigitizerStylusEvent(uint64_t timeStamp, IOHIDDigitizerStylusData * stylusData);
```

## Parameters 

`timeStamp`  

The timestamp of the event. Use the timestamp of the report element that is the source of the event.

`stylusData`  

A structure containing the stylus data. For more information, see IOHIDDigitizerStylusData.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Call this method from your event service to dispatch a stylus event to the system. Typically, you call this method when handling a report from the device, after you determine that the event originated from a stylus.

## See Also

### Dispatching Events to the System

dispatchDigitizerTouchEvent

Dispatches a digitizer touch event to the system.

