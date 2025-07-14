

- CFNetwork
-  CFHostClientContext 

Structure

# CFHostClientContext

A structure containing user-defined data and callbacks for CFHost objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
struct CFHostClientContext
```

## Topics

### Initializers

init()

Initializes an object that contains user-defined data and callbacks for a network host.

init(version: CFIndex, info: UnsafeMutableRawPointer?, retain: CFAllocatorRetainCallBack?, release: CFAllocatorReleaseCallBack?, copyDescription: CFAllocatorCopyDescriptionCallBack?)

Initializes an object that contains user-defined data and callbacks for a network host using the specified values.

### Instance Properties

var copyDescription: CFAllocatorCopyDescriptionCallBack?

The callback used to create a descriptive string representation of the info pointer (or the data pointed to by the info pointer) for debugging purposes. This callback is called by the CFCopyDescription(_:) function.

var info: UnsafeMutableRawPointer?

An arbitrary pointer to allocated memory containing user-defined data that can be associated with the host and that is passed to the callbacks.

var release: CFAllocatorReleaseCallBack?

The callback used to remove a retain previously added for the host on the info pointer.

var retain: CFAllocatorRetainCallBack?

The callback used to add a retain for the host on the info pointer for the life of the host, and may be used for temporary references the host needs to take. This callback returns the actual info pointer to store in the host, almost always just the pointer passed as the parameter.

var version: CFIndex

The version number of the structure type passed as a parameter to the host client function. The only valid version number is `0`.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Hosts

class CFHost

An opaque reference representing an CFHost object.

enum CFHostInfoType

Values indicating the type of data that is to be resolved or the type of data that was resolved.

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

func CFHostStartInfoResolution(CFHost, CFHostInfoType, UnsafeMutablePointer&lt;CFStreamError>?) -> Bool

Starts resolution for a host object.

Deprecated

func CFHostUnscheduleFromRunLoop(CFHost, CFRunLoop, CFString)

Unschedules a CFHost from a run loop.

Deprecated

