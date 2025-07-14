

- Paravirtualized Graphics
-  PGResumeErrorCode 

Enumeration

# PGResumeErrorCode

Error codes for suspend-resume actions.

Mac Catalyst 14.0+macOS 11.0+

``` source
enum PGResumeErrorCode
```

## Topics

### Errors

case incompatibleDevice

The resume device is missing capabilities that the suspended device provided.

case internalFault

An internal error occurred.

case invalidContent

The content of the suspend state or the guest memory isn’t valid.

case invalidGuestVersion

The guest version is incompatible with this framework version.

case invalidSuspendStateVersion

The suspend state version is incompatible with this framework version.

### Enumeration Cases

case invalidDisplayPortCount

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Suspending and Resuming Graphics Processing

func willSuspend()

Notifies the virtual graphics device to start suspending graphics activities.

**Required**

func finishSuspend() -> Data?

Notifies the virtualized graphics device to finish suspending graphics activities.

**Required**

func willResume(withSuspendState: Data, error: NSErrorPointer) -> Bool

Tells a new device object to load a previously saved device’s suspend state.

**Required**

func didResume()

Tells the device object to finish any remaining work to resume processing of a previously saved device’s suspend state.

**Required**

let PGResumeErrorDomain: String

The error domain for suspend-resume actions.

