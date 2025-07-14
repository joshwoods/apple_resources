

- CFNetwork
-  CFNetServiceCreate(\_:\_:\_:\_:\_:) Deprecated

Function

# CFNetServiceCreate(\_:\_:\_:\_:\_:)

Creates an instance of a Network Service object.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.2–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceCreate(
    _ alloc: CFAllocator?,
    _ domain: CFString,
    _ serviceType: CFString,
    _ name: CFString,
    _ port: Int32
) -> Unmanaged
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`domain`  

The domain in which the CFNetService is to be registered; cannot be `NULL`. Call CFNetServiceBrowserCreate(_:_:_:) and CFNetServiceBrowserSearchForDomains(_:_:_:) to get the registration domain.

`name`  

A unique name if the instance will be used to register a service. The name will become part of the instance name in the DNS records that will be created when the service is registered. If the instance will be used to resolve a service, the name should be the name of the machine or service that will be resolved.

`port`  

Local IP port, in host byte order, on which this service accepts connections. Pass zero to get placeholder service. With a placeholder service, the service will not be discovered by browsing, but a name conflict will occur if another client tries to register the same name. Most applications do not need to use placeholder service.

## Return Value

A new net service object, or `NULL` if the instance could not be created. Ownership follows the The Create Rule.

## Discussion

If the service depends on information in DNS TXT records, call `CFNetServiceSetProtocolSpecificInformation`.

If the CFNetService is to run in asynchronous mode, call CFNetServiceSetClient(_:_:_:) to prepare the service for running in asynchronous mode. Then call CFNetServiceScheduleWithRunLoop(_:_:_:) to schedule the service on a run loop. Then call CFNetServiceRegister to make the service available.

If the CFNetService is to run in synchronous mode, call CFNetServiceRegister.

To terminate a service that is running in asynchronous mode, call CFNetServiceCancel(_:) and CFNetServiceUnscheduleFromRunLoop(_:_:_:).

To terminate a service that is running in synchronous mode, call CFNetServiceCancel(_:).

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

