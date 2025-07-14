

- CFNetwork
-  CFNetServiceMonitorStart(\_:\_:\_:) Deprecated

Function

# CFNetServiceMonitorStart(\_:\_:\_:)

Starts monitoring.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.4–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceMonitorStart(
    _ monitor: CFNetServiceMonitor,
    _ recordType: CFNetServiceMonitorType,
    _ error: UnsafeMutablePointer?
) -> Bool
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`monitor`  

CFNetServiceMonitor, created by calling CFNetServiceMonitorCreate(_:_:_:_:), that is to be started.

`recordType`  

CFNetServiceMonitorType that specified the type of record to monitor. For possible values, see CFNetServiceMonitorType.

`error`  

Pointer to a CFStreamError structure. If an error occurs, on output, the structure’s `domain` field will be set to the error code’s domain and the `error` field will be set to an appropriate error code. Set this parameter to `NULL` if you don’t want to receive the error code and its domain.

## Return Value

`TRUE` if an asynchronous monitor was started successfully. `FALSE` if an error occurred when starting an asynchronous or synchronous monitor, or if CFNetServiceMonitorStop(_:_:) was called for an synchronous monitor.

## Discussion

This function starts monitoring for changes to records of the type specified by `recordType`. If a monitor is already running for the service associated with the specified CFNetServiceMonitorRef, this function returns `FALSE`.

For synchronous monitors, this function blocks until the monitor is stopped by calling CFNetServiceMonitorStop(_:_:), in which case, this function returns `FALSE`.

For asynchronous monitors, this function returns `TRUE` or `FALSE`, depending on whether monitoring starts successfully.

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

