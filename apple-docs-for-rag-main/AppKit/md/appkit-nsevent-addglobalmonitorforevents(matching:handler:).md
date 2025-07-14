

- AppKit
- NSEvent
-  addGlobalMonitorForEvents(matching:handler:) 

Type Method

# addGlobalMonitorForEvents(matching:handler:)

Installs an event monitor that receives copies of events the system posts to other applications.

macOS 10.6+

``` source
class func addGlobalMonitorForEvents(
    matching mask: NSEvent.EventTypeMask,
    handler block: @escaping (NSEvent) -> Void
) -> Any?
```

## Parameters 

`mask`  

An event mask specifying which events you wish to monitor. See NSEvent.EventTypeMask for possible values.

`block`  

The event handler block object. It is passed the event to monitor. You are unable to change the event, merely observe it.

## Return Value

An event handler object.

## Discussion

Events are delivered asynchronously to your app and you can only observe the event; you cannot modify or otherwise prevent the event from being delivered to its original target application.

Key-related events may only be monitored if accessibility is enabled or if your application is trusted for accessibility access (see AXIsProcessTrusted()).

Note that your handler will not be called for events that are sent to your own application.

### Special Considerations

In OS X v 10.6, event monitors are only able to monitor the following event types:

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

class func addLocalMonitorForEvents(matching: NSEvent.EventTypeMask, handler: (NSEvent) -> NSEvent?) -> Any?

Installs an event monitor that receives copies of events the system posts to this app prior to their dispatch.

class func removeMonitor(Any)

Removes the specified event monitor.

