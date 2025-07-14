

- CFNetwork
-  CFHostGetAddressing(\_:\_:) Deprecated

Function

# CFHostGetAddressing(\_:\_:)

Gets the addresses from a host.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.3–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFHostGetAddressing(
    _ theHost: CFHost,
    _ hasBeenResolved: UnsafeMutablePointer?
) -> Unmanaged?
```

Deprecated

Use Network framework instead, see deprecation notice in \

## Parameters 

`theHost`  

The CFHost whose addresses are to be obtained. This value must not be `NULL`.

`hasBeenResolved`  

On return, a pointer to a Boolean that is `TRUE` if addresses were available and `FALSE` if addresses were not available. This parameter can be null.

## Discussion

This function gets the addresses from a CFHost. The CFHost must have been previously resolved. To resolve a CFHost, call CFHostStartInfoResolution(_:_:_:).

### Special Considerations

This function gets the addresses in a thread-safe way, but the resulting data is not thread-safe. The data is returned as a “get” as opposed to a copy, so the data is not safe if the CFHost is altered from another thread.

## See Also

### Hosts

class CFHost

An opaque reference representing an CFHost object.

enum CFHostInfoType

Values indicating the type of data that is to be resolved or the type of data that was resolved.

struct CFHostClientContext

A structure containing user-defined data and callbacks for CFHost objects.

func CFHostCancelInfoResolution(CFHost, CFHostInfoType)

Cancels the resolution of a host.

Deprecated

func CFHostCreateCopy(CFAllocator?, CFHost) -> Unmanaged&lt;CFHost>

Creates a new host object by copying.

Deprecated

func CFHostCreateWithAddress(CFAllocator?, CFData) -> Unmanaged&lt;CFHost>

Uses an address to create an instance of a host object.

Deprecated

func CFHostCreateWithName(CFAllocator?, CFString) -> Unmanaged&lt;CFHost>

Uses a name to create an instance of a host object.

Deprecated

func CFHostGetNames(CFHost, UnsafeMutablePointer&lt;DarwinBoolean>?) -> Unmanaged&lt;CFArray>?

Gets the names from a CFHost.

Deprecated

func CFHostGetReachability(CFHost, UnsafeMutablePointer&lt;DarwinBoolean>?) -> Unmanaged&lt;CFData>?

Gets reachability information from a host.

Deprecated

func CFHostGetTypeID() -> CFTypeID

Gets the Core Foundation type identifier for the CFHost opaque type.

Deprecated

func CFHostScheduleWithRunLoop(CFHost, CFRunLoop, CFString)

Schedules a CFHost on a run loop.

Deprecated

func CFHostSetClient(CFHost, CFHostClientCallBack?, UnsafeMutablePointer&lt;CFHostClientContext>?) -> Bool

Associates a client context and a callback function with a CFHost object or disassociates a client context and callback function that were previously set.

Deprecated

func CFHostStartInfoResolution(CFHost, CFHostInfoType, UnsafeMutablePointer&lt;CFStreamError>?) -> Bool

Starts resolution for a host object.

Deprecated

func CFHostUnscheduleFromRunLoop(CFHost, CFRunLoop, CFString)

Unschedules a CFHost from a run loop.

Deprecated

