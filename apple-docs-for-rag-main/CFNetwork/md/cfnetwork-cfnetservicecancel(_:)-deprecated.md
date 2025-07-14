

- CFNetwork
-  CFNetServiceCancel(\_:) Deprecated

Function

# CFNetServiceCancel(\_:)

Cancels a service registration or a service resolution.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.2–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceCancel(_ theService: CFNetService)
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`theService`  

The CFNetService, obtained by previously calling CFNetServiceCreate(_:_:_:_:_:), for which a registration or a resolution is to be canceled.

## Discussion

This function cancels service registrations, started by CFNetServiceRegister, thereby making the service unavailable. It also cancels service resolutions, started by CFNetServiceResolve.

If you are shutting down an asynchronous service, you should first call CFNetServiceUnscheduleFromRunLoop(_:_:_:) and CFNetServiceSetClient(_:_:_:) with `clientCB` set to `NULL.` Then call this function.

If you are shutting down a synchronous service, call this function from another thread.

This function also cancels service resolutions. You would want to cancel a service resolution if your callback function has received an IP address that you’ve successfully used to connect to the service. In addition, you might want to cancel a service resolution if the resolution is taking longer than a user would want to wait or if the user canceled the operation.

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

