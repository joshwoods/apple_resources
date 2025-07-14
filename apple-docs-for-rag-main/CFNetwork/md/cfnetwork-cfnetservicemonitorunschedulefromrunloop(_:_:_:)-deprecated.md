

- CFNetwork
-  CFNetServiceMonitorUnscheduleFromRunLoop(\_:\_:\_:) Deprecated

Function

# CFNetServiceMonitorUnscheduleFromRunLoop(\_:\_:\_:)

Unschedules a CFNetServiceMonitor from a run loop.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.4–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceMonitorUnscheduleFromRunLoop(
    _ monitor: CFNetServiceMonitor,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
)
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`monitor`  

The CFNetServiceMonitor that is to be unscheduled; cannot be `NULL`.

`runLoop`  

The run loop; cannot be `NULL`.

`runLoopMode`  

The mode from which the monitor is to be unscheduled; cannot be `NULL`.

## Discussion

Unschedules the specified monitor from the specified run loop and mode. Call this function to shut down a monitor that is running asynchronously.

To change a monitor so that it cannot be scheduled and so that its callback will never be called, call CFNetServiceMonitorInvalidate(_:).

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

