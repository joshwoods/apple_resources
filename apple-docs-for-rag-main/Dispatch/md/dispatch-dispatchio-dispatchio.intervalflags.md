

- Dispatch
- DispatchIO
-  DispatchIO.IntervalFlags 

Structure

# DispatchIO.IntervalFlags

The desired delivery behavior for interval events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct IntervalFlags
```

## Topics

### Interval Flags

static let strictInterval: DispatchIO.IntervalFlags

Enqueue handlers for a channel at strict intervals regardless of how much data has been read or written.

var DISPATCH_IO_STRICT_INTERVAL: Int32

Enqueue handlers for a channel at strict intervals regardless of how much data has been read or written.

### Initializing the Type

init(nilLiteral: ())

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Managing the File Descriptor

var fileDescriptor: Int32

Returns the file descriptor associated with the specified channel.

func setLimit(highWater: Int)

Sets the maximum number of bytes to process before enqueueing a handler block.

func setLimit(lowWater: Int)

Sets the minimum number of bytes to process before enqueueing a handler block.

func setInterval(interval: DispatchTimeInterval, flags: DispatchIO.IntervalFlags)

Sets the interval, in nanoseconds, at which to invoke the I/O handlers for the channel.

