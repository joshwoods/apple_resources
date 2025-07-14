

- CFNetwork
-  CFHostStartInfoResolution(\_:\_:\_:) Deprecated

Function

# CFHostStartInfoResolution(\_:\_:\_:)

Starts resolution for a host object.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.3–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFHostStartInfoResolution(
    _ theHost: CFHost,
    _ info: CFHostInfoType,
    _ error: UnsafeMutablePointer?
) -> Bool
```

Deprecated

Use Network framework instead, see deprecation notice in \

## Parameters 

`theHost`  

The host, obtained by previously calling CFHostCreateCopy(_:_:), CFHostCreateWithAddress(_:_:), or CFHostCreateWithName(_:_:), that is to be resolved. This value must not be `NULL`.

`info`  

A value of type `CFHostInfoType` specifying the type of information that is to be retrieved. See CFHostInfoType for possible values.

`error`  

A pointer to a CFStreamError structure, that, if an error occurs, is set to the error and the error’s domain. In synchronous mode, the error indicates why resolution failed, and in asynchronous mode, the error indicates why resolution failed to start.

## Return Value

`TRUE` if the resolution was started (asynchronous mode); `FALSE` if another resolution is already in progress for `theHost` or if an error occurred.

## Discussion

This function retrieves the information specified by `info` and stores it in the host.

In synchronous mode, this function blocks until the resolution has completed, in which case this function returns `TRUE`, until the resolution is stopped by calling CFHostCancelInfoResolution(_:_:) from another thread, in which case this function returns `FALSE`, or until an error occurs.

### Special Considerations

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

func CFHostCreateCopy(CFAllocator?, CFHost) -> Unmanaged&lt;CFHost>

Creates a new host object by copying.

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

func CFHostUnscheduleFromRunLoop(CFHost, CFRunLoop, CFString)

Unschedules a CFHost from a run loop.

Deprecated

