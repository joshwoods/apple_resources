

- IOUSBHost
-  IOUSBHostObject 

Class

# IOUSBHostObject

This class provides basic functionality for sending device requests and retrieving descriptors.

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostObject
```

## Topics

### Managing the Object Life Cycle

struct IOUSBHostObjectInitOptions

Options for initializing the host object.

typealias IOUSBHostInterestHandler

The callback that handles underlying service-state changes.

var ioService: io_service_t

A reference to the kernel object.

var queue: dispatch_queue_t

The queue for servicing input/output requests.

func destroy()

Removes underlying allocations and connections from the USB host object.

### Retrieving Base Class Descriptors

Parsing USB Descriptors

Extract information from various USB descriptors using helper methods.

### Creating I/O Buffers

func ioData(withCapacity: Int) throws -> NSMutableData

Allocates a buffer for input/output requests.

### Sending Device Requests

func IOUSBHostDeviceRequestType(tIOUSBDeviceRequestDirectionValue, tIOUSBDeviceRequestTypeValue, tIOUSBDeviceRequestRecipientValue) -> UInt8

Creates the request type field of a device request.

let IOUSBHostDefaultControlCompletionTimeout: TimeInterval

The default completion timeout for input/output requests.

### Enqueueing Device Requests

typealias IOUSBHostCompletionHandler

The completion handler for asynchronous control, bulk, and interrupt transfers.

### Aborting Device Requests

enum IOUSBHostAbortOption

Options for aborting pending input/output requests.

### Getting Host Information

var deviceAddress: Int

The device’s bus address.

### Instance Properties

var capabilityDescriptors: UnsafePointer&lt;IOUSBBOSDescriptor>?

var deviceDescriptor: UnsafePointer&lt;IOUSBDeviceDescriptor>?

### Instance Methods

func configurationDescriptor(with: Int) throws -> UnsafePointer&lt;IOUSBConfigurationDescriptor>

func configurationDescriptor(withConfigurationValue: Int) throws -> UnsafePointer&lt;IOUSBConfigurationDescriptor>

func destroy(options: IOUSBHostObjectDestroyOptions)

### Related Documentation

class IOUSBHostDevice

The class that claims and configures devices, retrieves descriptors, and sends device requests.

class IOUSBHostInterface

The class for accessing USB-related services.

## Relationships

### Inherits From

- NSObject

### Inherited By

- IOUSBHostDevice
- IOUSBHostInterface

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Base Classes

class IOUSBHostIOSource

This class provides basic functionality for deriving pipe and stream classes.

