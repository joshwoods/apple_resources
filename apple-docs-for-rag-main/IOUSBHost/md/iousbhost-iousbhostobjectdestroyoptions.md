

- IOUSBHost
-  IOUSBHostObjectDestroyOptions 

Structure

# IOUSBHostObjectDestroyOptions

Mac Catalyst 14.0+macOS 10.15+

``` source
struct IOUSBHostObjectDestroyOptions
```

## Overview

```
          the device will not be reset and drivers will not be re-registered for matching.  This allows for IOUSBHostDevice
          objects that were initialized with IOUSBHostObjectInitOptionsDeviceCapture to honor the
          kUSBHostMessageDeviceIsRequestingClose message.

          This option is only valid for macOS
```

## Topics

### Initializers

init(rawValue: UInt)

### Type Properties

static var deviceSurrender: IOUSBHostObjectDestroyOptions

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

### Structures

struct IOUSBHostCIControllerState

struct IOUSBHostCIDeviceSpeed

struct IOUSBHostCIDeviceState

struct IOUSBHostCIEndpointState

struct IOUSBHostCIExceptionType

struct IOUSBHostCILinkState

struct IOUSBHostCIMessage

struct IOUSBHostCIMessageStatus

struct IOUSBHostCIMessageType

struct IOUSBHostCIPortState

struct IOUSBHostCIUserClientVersion

struct IOUSBHostIsochronousTransaction

struct IOUSBHostIsochronousTransactionOptions

struct IOUSBHostIsochronousTransferOptions

