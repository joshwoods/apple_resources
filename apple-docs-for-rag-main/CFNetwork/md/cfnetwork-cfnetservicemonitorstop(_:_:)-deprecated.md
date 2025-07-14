

- CFNetwork
-  CFNetServiceMonitorStop(\_:\_:) Deprecated

Function

# CFNetServiceMonitorStop(\_:\_:)

Stops a CFNetServiceMonitor.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.4–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceMonitorStop(
    _ monitor: CFNetServiceMonitor,
    _ error: UnsafeMutablePointer?
)
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`monitor`  

CFNetServiceMonitor, started by calling CFNetServiceMonitorStart(_:_:_:), that is to be stopped.

`error`  

Pointer to a CFStreamError structure or `NULL`. For synchronous monitors, set the `error` field of this structure to the non-zero value you want to be set in the `CFStreamError` structure when CFNetServiceMonitorStart(_:_:_:) returns. Note that when it returns, CFNetServiceMonitorStart(_:_:_:) returns `FALSE.` If the monitor was started asynchronously, set the `error` field to the non-zero value you want the monitor’s callback to receive when it is called. If this parameter is `NULL`, default values for the `CFStreamError` structure are used: the domain is set to `kCFStreamErrorDomainNetServices` and the error code is set to `kCFNetServicesErrorCancel`.

## Discussion

This function stops the specified monitor. Call CFNetServiceMonitorStart(_:_:_:) if you want to start monitoring again.

If you want to stop monitoring and no longer need to monitor record changes, call CFNetServiceMonitorInvalidate(_:) instead of this function.

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

