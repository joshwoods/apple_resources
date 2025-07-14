

- HIDDriverKit
- IOUserHIDEventService
-  dispatchEvent 

Instance Method

# dispatchEvent

Dispatches a HID event to the system.

DriverKit 19.0+macOS

``` source
void dispatchEvent(IOHIDEvent * event);
```

## Parameters 

`event`  

The event to dispatch.

## Discussion

This method is a funnel point for dispatching events to the system’s registered clients. You can also call it directly to dispatch events for which you create an `IOHIDEvent` object.

## See Also

### Performing Private Tasks

createReportPool

