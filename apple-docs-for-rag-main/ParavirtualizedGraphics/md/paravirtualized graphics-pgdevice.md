

- Paravirtualized Graphics
-  PGDevice 

Protocol

# PGDevice

A paravirtualized GPU device object.

Mac Catalyst 14.0+macOS 11.0+

``` source
protocol PGDevice : NSObjectProtocol
```

## Topics

### Handling Memory-Mapped I/O

func mmioRead(atOffset: Int) -> UInt32

Reads data from the virtual graphics device’s memory-mapped I/O region.

**Required**

func mmioWrite(atOffset: Int, value: UInt32)

Writes data to the virtual graphics device’s memory-mapped I/O region.

**Required**

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

enum PGResumeErrorCode

Error codes for suspend-resume actions.

### Managing Displays

func newDisplay(with: PGDisplayDescriptor, port: Int, serialNum: UInt32) -> (any PGDisplay)?

Create a display from the specified descriptor and uniquifying parameters.

**Required**

### Instance Methods

func pause()

**Required**

func reset()

**Required**

func stop()

**Required**

func unpause()

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Devices

func PGNewDeviceWithDescriptor(PGDeviceDescriptor) -> (any PGDevice)?

Creates a new paravirtualized graphics device.

class PGDeviceDescriptor

A description of the paravirtualized graphics device to create.

