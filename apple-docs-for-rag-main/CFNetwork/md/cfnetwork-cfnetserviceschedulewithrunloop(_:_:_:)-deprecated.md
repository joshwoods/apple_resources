

- CFNetwork
-  CFNetServiceScheduleWithRunLoop(\_:\_:\_:) Deprecated

Function

# CFNetServiceScheduleWithRunLoop(\_:\_:\_:)

Schedules a CFNetService on a run loop.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.2–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceScheduleWithRunLoop(
    _ theService: CFNetService,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
)
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`theService`  

The CFNetService that is to be scheduled on a run loop; cannot be `NULL`.

`runLoop`  

The run loop on which the service is to be scheduled; cannot be `NULL`.

`runLoopMode`  

The mode on which to schedule the service; cannot be `NULL`.

## Discussion

Schedules the specified service on a run loop, which places the service in asynchronous mode. The caller is responsible for ensuring that at least one of the run loops on which the service is scheduled is being run.

### Special Considerations

This function is thread safe.

Before calling this function, call CFNetServiceSetClient(_:_:_:) to prepare a CFNetService for use in asynchronous mode.

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

