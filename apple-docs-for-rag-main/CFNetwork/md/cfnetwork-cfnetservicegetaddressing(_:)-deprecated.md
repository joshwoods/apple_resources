

- CFNetwork
-  CFNetServiceGetAddressing(\_:) Deprecated

Function

# CFNetServiceGetAddressing(\_:)

Gets the IP addressing from a CFNetService.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.2–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceGetAddressing(_ theService: CFNetService) -> Unmanaged?
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`theService`  

The CFNetService whose IP addressing is to be obtained; cannot be `NULL`.

## Return Value

A CFArray containing a CFDataRef for each IP address returned, or `NULL`. Each CFDataRef consists of a `sockaddr` structure containing the IP address of the service. This function returns `NULL` if the service’s addressing is unknown because CFNetServiceResolve has not been called for `theService`.

## Discussion

This function gets the IP addressing from a CFNetService. Typically, the CFNetService was obtained by calling CFNetServiceBrowserSearchForServices(_:_:_:_:). Before calling this function, call CFNetServiceResolve to update the CFNetService with its IP addressing.

### Special Considerations

This function gets the data in a thread-safe way, but the data itself is not safe if the service is altered from another thread.

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

