

- CFNetwork
-  CFNetServiceBrowserStopSearch(\_:\_:) Deprecated

Function

# CFNetServiceBrowserStopSearch(\_:\_:)

Stops a search for domains or services.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.2–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceBrowserStopSearch(
    _ browser: CFNetServiceBrowser,
    _ error: UnsafeMutablePointer?
)
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`browser`  

The CFNetServiceBrowser that was used to start the search; cannot be `NULL`.

`error`  

A pointer to a CFStreamError structure that will be passed to the callback function associated with this CFNetServiceBrowser (if the search is being conducted in asynchronous mode) or that is pointed to by the `error` parameter when CFNetServiceBrowserSearchForDomains(_:_:_:) or CFNetServiceBrowserSearchForServices(_:_:_:_:) returns (if the search is being conducted in synchronous mode). Set the `domain` field to `kCFStreamErrorDomainCustom` and the `error` field to an appropriate value.

## Discussion

This functions stops a search started by a previous call to CFNetServiceBrowserSearchForDomains(_:_:_:) or CFNetServiceBrowserSearchForServices(_:_:_:_:). For asynchronous and synchronous searches, calling this function causes the callback function associated with the CFNetServiceBrowser to be called once for each domain or service found. If the search is asynchronous, `error` is passed to the callback function. If the search is synchronous, calling this function causes CFNetServiceBrowserSearchForDomains(_:_:_:) or CFNetServiceBrowserSearchForServices(_:_:_:_:) to return `FALSE`. If the `error` parameter for either call pointed to a CFStreamError structure, the CFStreamError structure contains the error code and the error code’s domain as set when this function was called.

### Special Considerations

This function is thread safe.

If you are stopping an asynchronous search, before calling this function, call CFNetServiceBrowserUnscheduleFromRunLoop(_:_:_:), followed by CFNetServiceBrowserInvalidate(_:).

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

func CFNetServiceBrowserUnscheduleFromRunLoop(CFNetServiceBrowser, CFRunLoop, CFString)

Unschedules a CFNetServiceBrowser from a run loop and mode.

Deprecated

