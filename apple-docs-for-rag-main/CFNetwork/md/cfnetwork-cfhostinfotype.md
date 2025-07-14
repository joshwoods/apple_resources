

- CFNetwork
-  CFHostInfoType 

Enumeration

# CFHostInfoType

Values indicating the type of data that is to be resolved or the type of data that was resolved.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
enum CFHostInfoType
```

## Topics

### Constants

case addresses

Specifies that addresses are to be resolved or that addresses were resolved.

case names

Specifies that names are to be resolved or that names were resolved.

case reachability

Specifies that reachability information is to be resolved or that reachability information was resolved.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Hosts

class CFHost

An opaque reference representing an CFHost object.

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

func CFHostStartInfoResolution(CFHost, CFHostInfoType, UnsafeMutablePointer&lt;CFStreamError>?) -> Bool

Starts resolution for a host object.

Deprecated

func CFHostUnscheduleFromRunLoop(CFHost, CFRunLoop, CFString)

Unschedules a CFHost from a run loop.

Deprecated

