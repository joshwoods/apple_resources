

- CFNetwork
-  CFNetServiceSetClient(\_:\_:\_:) Deprecated

Function

# CFNetServiceSetClient(\_:\_:\_:)

Associates a callback function with a CFNetService or disassociates a callback function from a CFNetService.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.2–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceSetClient(
    _ theService: CFNetService,
    _ clientCB: CFNetServiceClientCallBack?,
    _ clientContext: UnsafeMutablePointer?
) -> Bool
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`theService`  

The CFNetService; cannot be `NULL`.

`clientCB`  

The callback function that is to be associated with this CFNetService. If you are shutting down the service, set `clientCB` to `NULL` to disassociate from this CFNetService the callback function that was previously associated.

`clientContext`  

Context information to be used when `clientCB` is called; cannot be `NULL`.

## Return Value

`TRUE` if the client was set; otherwise, `FALSE`.

## Discussion

The callback function specified by `clientCB` will be called to report IP addresses (in the case of CFNetServiceResolve) or to report registration errors (in the case of CFNetServiceRegister).

### Special Considerations

This function is thread safe.

For a CFNetService that will operate asynchronously, call this function and then call CFNetServiceScheduleWithRunLoop(_:_:_:) to schedule the service on a run loop. Then call CFNetServiceRegister or CFNetServiceResolve.

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

