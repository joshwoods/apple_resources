

- CFNetwork
-  CFNetServiceMonitorCreate(\_:\_:\_:\_:) Deprecated

Function

# CFNetServiceMonitorCreate(\_:\_:\_:\_:)

Creates an instance of a NetServiceMonitor object that watches for record changes.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.4–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceMonitorCreate(
    _ alloc: CFAllocator?,
    _ theService: CFNetService,
    _ clientCB: CFNetServiceMonitorClientCallBack,
    _ clientContext: UnsafeMutablePointer
) -> Unmanaged
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theService`  

CFNetService to be monitored.

`clientCB`  

Pointer to callback function that is to be called when a record associated with `theService` changes; cannot be `NULL`.

`clientContext`  

Pointer to user-defined contextual information that is to be passed to the callback specified by `clientCB` when the callback is called; cannot be `NULL`. For details, see CFNetServiceClientContext.

## Return Value

A new instance of a CFNetServiceMonitor, or `NULL` if the monitor could not be created. Ownership follows the The Create Rule.

## Discussion

This function creates a CFNetServiceMonitor that watches for changes in records associated with `theService`.

If the CFNetServiceMonitor is to run in asynchronous mode, call CFNetServiceMonitorScheduleWithRunLoop(_:_:_:) to schedule the monitor on a run loop. Then call CFNetServiceMonitorStart(_:_:_:) to start monitoring. When a change occurs, the callback function specified by `clientCB` will be called. For details, see CFNetServiceMonitorClientCallBack.

If the CFNetServiceMonitor is to run in synchronous mode, call CFNetServiceMonitorStart(_:_:_:).

To stop a monitor that is running in asynchronous mode, call CFNetServiceMonitorStop(_:_:) and CFNetServiceMonitorUnscheduleFromRunLoop(_:_:_:).

To stop a monitor that is running in synchronous mode, call CFNetServiceMonitorStop(_:_:).

If you no longer need to monitor record changes, call CFNetServiceMonitorStop(_:_:) to stop the monitor and then call CFNetServiceMonitorInvalidate(_:)to invalidate the monitor so it cannot be used again. Then call `CFRelease` to release the memory associated with CFNetServiceMonitorRef.

### Special Considerations

This function is thread safe.

## See Also

### Network Services

class CFNetService

An opaque reference representing a CFNetService.

class CFNetServiceBrowser

An opaque reference representing a CFNetServiceBrowser.

struct CFNetServiceBrowserFlags

Flags that the system passes to net service browser callbacks.

class CFNetServiceMonitor

An opaque reference for a service monitor.

enum CFNetServiceMonitorType

Record type specifier used to tell a service monitor the type of record changes to watch for.

struct CFNetServiceClientContext

A structure provided when a CFNetService is associated with a callback function or when a CFNetServiceBrowser is created.

struct CFNetServiceRegisterFlags

Options to use when registering a service on the network.

enum CFNetServicesError

Error codes that may be returned by CFNetServices functions or passed to CFNetServices callback functions.

func CFNetServiceBrowserInvalidate(CFNetServiceBrowser)

Invalidates an instance of a Network Service browser object.

Deprecated

func CFNetServiceBrowserScheduleWithRunLoop(CFNetServiceBrowser, CFRunLoop, CFString)

Schedules a CFNetServiceBrowser on a run loop.

Deprecated

func CFNetServiceBrowserCreate(CFAllocator?, CFNetServiceBrowserClientCallBack, UnsafeMutablePointer&lt;CFNetServiceClientContext>) -> Unmanaged&lt;CFNetServiceBrowser>

Creates an instance of a Network Service browser object.

Deprecated

func CFNetServiceBrowserGetTypeID() -> CFTypeID

Gets the Core Foundation type identifier for the Network Service browser object.

Deprecated

func CFNetServiceBrowserSearchForDomains(CFNetServiceBrowser, Bool, UnsafeMutablePointer&lt;CFStreamError>?) -> Bool

Searches for domains.

Deprecated

func CFNetServiceBrowserSearchForServices(CFNetServiceBrowser, CFString, CFString, UnsafeMutablePointer&lt;CFStreamError>?) -> Bool

Searches a domain for services of a specified type.

Deprecated

func CFNetServiceBrowserStopSearch(CFNetServiceBrowser, UnsafeMutablePointer&lt;CFStreamError>?)

Stops a search for domains or services.

Deprecated

