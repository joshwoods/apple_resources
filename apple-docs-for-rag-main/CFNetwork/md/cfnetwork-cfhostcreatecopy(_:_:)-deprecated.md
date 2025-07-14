

- CFNetwork
-  CFHostCreateCopy(\_:\_:) Deprecated

Function

# CFHostCreateCopy(\_:\_:)

Creates a new host object by copying.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.3–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFHostCreateCopy(
    _ alloc: CFAllocator?,
    _ host: CFHost
) -> Unmanaged
```

Deprecated

Use Network framework instead, see deprecation notice in \

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

## Return Value

A valid CFHost object or `NULL` if the copy could not be created. The new host contains a copy of all previously resolved data from the original host. Ownership follows the The Create Rule.

## Discussion

This function is thread safe.

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

func CFHostCreateWithAddress(CFAllocator?, CFData) -> Unmanaged&lt;CFHost>

Uses an address to create an instance of a host object.

Deprecated

func CFHostCreateWithName(CFAllocator?, CFString) -> Unmanaged&lt;CFHost>

Uses a name to create an instance of a host object.

Deprecated

func CFHostGetAddressing(CFHost, UnsafeMutablePointer&lt;DarwinBoolean>?) -> Unmanaged&lt;CFArray>?

Gets the addresses from a host.

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

