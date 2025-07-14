

- IOUSBHost
-  IOUSBHostObjectInitOptions 

Structure

# IOUSBHostObjectInitOptions

Options for initializing the host object.

Mac Catalyst 14.0+macOS 10.15+

``` source
struct IOUSBHostObjectInitOptions
```

## Topics

### Options

static var deviceCapture: IOUSBHostObjectInitOptions

The option to capture the device and terminate existing drivers.

### Initializing the Structure

init(rawValue: UInt)

Initializes the object.

### Type Properties

static var deviceSeize: IOUSBHostObjectInitOptions

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

### Managing the Object Life Cycle

typealias IOUSBHostInterestHandler

The callback that handles underlying service-state changes.

var ioService: io_service_t

A reference to the kernel object.

var queue: dispatch_queue_t

The queue for servicing input/output requests.

func destroy()

Removes underlying allocations and connections from the USB host object.

