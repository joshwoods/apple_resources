

- AppKit
- NSEvent
-  addLocalMonitorForEvents(matching:handler:) 

Type Method

# addLocalMonitorForEvents(matching:handler:)

Installs an event monitor that receives copies of events the system posts to this app prior to their dispatch.

macOS 10.6+

``` source
class func addLocalMonitorForEvents(
    matching mask: NSEvent.EventTypeMask,
    handler block: @escaping (NSEvent) -> NSEvent?
) -> Any?
```

## Parameters 

`mask`  

An event mask specifying which events you wish to monitor. See NSEvent.EventTypeMask for possible values.

`block`  

The event handler block object. It is passed the event to monitor. You can return the event unmodified, create and return a new NSEvent object, or return nil to stop the dispatching of the event.

## Return Value

An event handler object.

## Discussion

Your handler will not be called for events that are consumed by nested event-tracking loops such as control tracking, menu tracking, or window dragging; only events that are dispatched through the applications sendEvent(_:) method will be passed to your handler.

Note

The monitor Block is called for all future events that match `mask`. You must call removeMonitor(_:) to stop the monitor.

### Special Considerations

In OS X v 10.6, event monitors are only able to monitor the following event types:

- NSFlagsChanged

- NSLeftMouseDragged

- NSRightMouseDragged

- NSOtherMouseDragged

- NSLeftMouseUp

- NSRightMouseUp

- NSOtherMouseUp

- NSLeftMouseDown

- NSRightMouseDown

- NSOtherMouseDown

- NSMouseMoved

- NSFlagsChanged

- NSScrollWheel

- NSTabletPoint

- NSTabletProximity

- NSKeyDown (Key repeats are determined using the isARepeat property.)

## See Also

### Monitoring app events

class func addGlobalMonitorForEvents(matching: NSEvent.EventTypeMask, handler: (NSEvent) -> Void) -> Any?

Installs an event monitor that receives copies of events the system posts to other applications.

class func removeMonitor(Any)

Removes the specified event monitor.

