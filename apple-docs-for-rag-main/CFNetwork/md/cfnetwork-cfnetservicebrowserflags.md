

- CFNetwork
-  CFNetServiceBrowserFlags 

Structure

# CFNetServiceBrowserFlags

Flags that the system passes to net service browser callbacks.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
struct CFNetServiceBrowserFlags
```

## Topics

### Constants

init(rawValue: CFOptionFlags)

Initializes a flag value with the specified bitfield.

### Type Properties

static var isDefault: CFNetServiceBrowserFlags

Specifies whether the resulting domain is the default registration or browse domain.

static var isDomain: CFNetServiceBrowserFlags

Specifies whether the result pertains to a search for domains or services.

static var isRegistrationDomain: CFNetServiceBrowserFlagsDeprecated

static var moreComing: CFNetServiceBrowserFlags

A hint that the system will call the client’s callback function again soon.

static var remove: CFNetServiceBrowserFlags

Specifies whether the client should remove the result instead of adding it.

static var isRegistrationDomain: CFNetServiceBrowserFlagsDeprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Network Services

class CFNetService

An opaque reference representing a CFNetService.

class CFNetServiceBrowser

An opaque reference representing a CFNetServiceBrowser.

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

func CFNetServiceBrowserUnscheduleFromRunLoop(CFNetServiceBrowser, CFRunLoop, CFString)

Unschedules a CFNetServiceBrowser from a run loop and mode.

Deprecated

