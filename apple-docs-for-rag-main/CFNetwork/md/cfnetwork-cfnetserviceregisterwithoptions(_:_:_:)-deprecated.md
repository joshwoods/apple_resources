

- CFNetwork
-  CFNetServiceRegisterWithOptions(\_:\_:\_:) Deprecated

Function

# CFNetServiceRegisterWithOptions(\_:\_:\_:)

Makes a CFNetService available on the network.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.4–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceRegisterWithOptions(
    _ theService: CFNetService,
    _ options: CFOptionFlags,
    _ error: UnsafeMutablePointer?
) -> Bool
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`theService`  

Network service to register; cannot be `NULL`. The registration will fail if the service doesn’t have a domain, a type, a name, and an IP address.

`options`  

Bit flags for specifying registration options. Currently, the only registration option is `kCFNetServiceFlagNoAutoRename`. For details, see `CFNetService Registration Options`.

`error`  

Pointer to a CFStreamError structure that will be set to an error code and the error code’s domain if an error occurs; or `NULL` if you don’t want to receive the error code and its domain.

## Return Value

`TRUE` if an asynchronous service registration was started; `FALSE` if an asynchronous or synchronous registration failed or if a synchronous registration was canceled.

## Discussion

If the service is to run in asynchronous mode, you must call CFNetServiceSetClient(_:_:_:) to associate a callback function with this CFNetService before calling this function.

When registering a service that runs in asynchronous mode, this function returns `TRUE` if the service contains all of the required attributes and the registration process can start. If the registration process completes successfully, the service is available on the network until you shut down the service by calling CFNetServiceUnscheduleFromRunLoop(_:_:_:), CFNetServiceSetClient(_:_:_:), and CFNetServiceCancel(_:). If the service does not contain all of the required attributes or if the registration process does not complete successfully, this function returns `FALSE`.

When registering a service that runs in synchronous mode, this function blocks until an error occurs, in which case this function returns `FALSE`. Until this function returns `FALSE`, the service is available on the network. To force this function to return `FALSE`, thereby shutting down the service, call CFNetServiceCancel(_:) from another thread.

The `options` parameter is a bit flag for specifying service registration options. Currently, `kCFNetServiceFlagNoAutoRename` is the only supported registration option. If this bit is set and a service of the same name is running, the registration will fail. If this bit is not set and a service of the same name is running, the service that is being registered will be renamed automatically by appending `(`*n*`)` to the service name, where *n* is a number that is incremented until the service can be registered with a unique name.

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

