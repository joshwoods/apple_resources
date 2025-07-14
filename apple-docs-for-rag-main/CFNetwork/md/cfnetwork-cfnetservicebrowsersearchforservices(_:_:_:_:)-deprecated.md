

- CFNetwork
-  CFNetServiceBrowserSearchForServices(\_:\_:\_:\_:) Deprecated

Function

# CFNetServiceBrowserSearchForServices(\_:\_:\_:\_:)

Searches a domain for services of a specified type.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.2–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceBrowserSearchForServices(
    _ browser: CFNetServiceBrowser,
    _ domain: CFString,
    _ serviceType: CFString,
    _ error: UnsafeMutablePointer?
) -> Bool
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`browser`  

The CFNetServiceBrowser, obtained by previously calling CFNetServiceBrowserCreate(_:_:_:), that is to perform the search; cannot be `NULL`.

`domain`  

The domain to search for the service type; cannot be `NULL`. To get the domains that are available for searching, call CFNetServiceBrowserSearchForDomains(_:_:_:).

`error`  

A pointer to a CFStreamError structure, that, if an error occurs, will be set to the error and the error’s domain and passed to your callback function. Pass `NULL` if you don’t want to receive the error that may occur as a result of this particular call.

## Return Value

`TRUE` if the search was started (asynchronous mode); `FALSE` if another search is already in progress for this CFNetServiceBrowser or if an error occurred.

## Discussion

This function searches the specified domain for services that match the specified service type. The search continues until the search is canceled by calling CFNetServiceBrowserStopSearch(_:_:). When a match is found, the callback function specified when the CFNetServiceBrowser was created is called and passed an instance of a CFNetService representing the service that was found.

In asynchronous mode, this function returns `TRUE` if the search was started. Otherwise, it returns `FALSE`.

In synchronous mode, this function blocks until the search is stopped by calling CFNetServiceBrowserStopSearch(_:_:) from another thread, in which case this function returns `FALSE`, or until an error occurs.

### Special Considerations

This function is thread safe.

For any one CFNetServiceBrowser, only one domain search or one service search can be in progress at the same time.

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

func CFNetServiceBrowserStopSearch(CFNetServiceBrowser, UnsafeMutablePointer&lt;CFStreamError>?)

Stops a search for domains or services.

Deprecated

func CFNetServiceBrowserUnscheduleFromRunLoop(CFNetServiceBrowser, CFRunLoop, CFString)

Unschedules a CFNetServiceBrowser from a run loop and mode.

Deprecated

