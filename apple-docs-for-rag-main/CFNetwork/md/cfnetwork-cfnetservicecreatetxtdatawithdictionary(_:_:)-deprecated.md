

- CFNetwork
-  CFNetServiceCreateTXTDataWithDictionary(\_:\_:) Deprecated

Function

# CFNetServiceCreateTXTDataWithDictionary(\_:\_:)

Flattens a set of key/value pairs into a CFDataRef suitable for passing to CFNetServiceSetTXTData(_:_:).

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.4–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFNetServiceCreateTXTDataWithDictionary(
    _ alloc: CFAllocator?,
    _ keyValuePairs: CFDictionary
) -> Unmanaged?
```

Deprecated

Use nw_browser_t or nw_listener_t in Network framework instead

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`keyValuePairs`  

CFDictionaryRef containing the key/value pairs that are to be placed in a TXT record. Each key must be a CFStringRef and each value should be a CFDataRef or a CFStringRef. (See the discussion below for additional information about values that are CFStringRefs.) This function fails if any other data types are provided. The length of a key and its value should not exceed 255 bytes.

## Return Value

A CFData object containing the flattened form of `keyValuePairs`, or `NULL` if the dictionary could not be flattened. Ownership follows the The Create Rule.

## Discussion

This function flattens the key/value pairs in the dictionary specified by `keyValuePairs` into a CFDataRef suitable for passing to CFNetServiceSetTXTData(_:_:). Note that this function is not a general purpose function for flattening CFDictionaryRefs.

The keys in the dictionary referenced by `keyValuePairs` must be CFStringRefs and the values must be CFDataRefs. Any values that are CFStringRefs are converted to CFDataRefs representing the flattened UTF-8 bytes of the string. The types of the values are not encoded in the CFDataRefs, so any CFStringRefs that are converted to CFDataRefs remain CFDataRefs when the CFDataRef produced by this function is processed by CFNetServiceCreateDictionaryWithTXTData(_:_:).

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

