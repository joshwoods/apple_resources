

- AppKit
- NSEvent
-  removeMonitor(\_:) 

Type Method

# removeMonitor(\_:)

Removes the specified event monitor.

macOS 10.6+

``` source
class func removeMonitor(_ eventMonitor: Any)
```

## Parameters 

`eventMonitor`  

The event handler object to remove.

## Discussion

You must ensure that `eventMonitor` is removed only once. Removing the same `eventMonitor` instance multiple times results in an over-release condition, even in a Garbage Collected environment

## See Also

### Monitoring app events

class func addGlobalMonitorForEvents(matching: NSEvent.EventTypeMask, handler: (NSEvent) -> Void) -> Any?

Installs an event monitor that receives copies of events the system posts to other applications.

class func addLocalMonitorForEvents(matching: NSEvent.EventTypeMask, handler: (NSEvent) -> NSEvent?) -> Any?

Installs an event monitor that receives copies of events the system posts to this app prior to their dispatch.

